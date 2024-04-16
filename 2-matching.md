# Task 2: Improve the matching algorithm

## Related issues:

* https://github.com/harmonydata/app/issues/14
* https://github.com/harmonydata/app/issues/15
* https://github.com/harmonydata/harmonyapi/issues/4
* https://github.com/harmonydata/harmony/issues/22
  
Harmony often matches items that should not be matched, or vice versa, e.g.

*Feeling tired or having little energy?* was incorrectly matched to *Having upsetting dreams that replay part of the experience or are clearly related to the experience?*

We have a Github repo where we have experimented with this: https://github.com/harmonydata/matching 

So how can we improve the matching? 

* Probably the easiest way would be to switch this underlying model, rather than trying anything clever.
* Longer term an LLM could be fine-tuned but that needs lots of resources and lots of data!

There are three ways you could run an LLM:

1. run an LLM on a server. For example, we can try different LLMs from HuggingFace Sentence Transformers
2. Add integration to OpenAI or Vertex (OpenAI example: https://github.com/harmonydata/matching/blob/main/03_ada3.py  Vertex example: https://github.com/harmonydata/matching/blob/main/06_google_vertex_ai_gecko_multilingual.py). This has the advantage that we don't need a server, but the disadvantage that we need to pay for the API key, and the third parties like OpenAI change their APIs quite frequently.
3. Run the LLM in the browser (on client side). Tensorflow JS model in the front end (https://github.com/tensorflow/tfjs-models Universal Sentence Encoder). I have a demo of TensorFlow JS Sentence Transformer here: https://fastdatascience.com/semantic-similarity-with-sentence-embeddings/

Check the code samples here for data and examples: https://github.com/harmonydata/matching 

Check this blog post too: https://harmonydata.ac.uk/measuring-the-performance-of-nlp-algorithms/

## Data

We have been evaluating the matching using the manually created harmonisation tool by McElroy et al. So where human annotators considered two items to be similar and Harmony also did, it gets points. Where Harmony disagreed with human annotators it scores lower. Here is the evaluation dataset in Excel form, which is used in the `matching` repository:

https://github.com/harmonydata/harmony_original/blob/main/data/Final%20harmonised%20item%20tool%20EM.xlsx


# Code snippets


Here is an example HTML file using the https://github.com/tensorflow/tfjs-models Universal Sentence Encoder

```

<html>
<head>
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs"></script>
<script src="https://cdn.jsdelivr.net/npm/@tensorflow-models/universal-sentence-encoder"></script>
</head>

<body>

<script>
// Load the model.
use.loadQnA().then(model => {
  // Embed a dictionary of a query and responses. The input to the embed method
  // needs to be in following format:
  // {
  //   queries: string[];
  //   responses: Response[];
  // }
  // queries is an array of question strings
  // responses is an array of following structure:
  // {
  //   response: string;
  //   context?: string;
  // }
  // context is optional, it provides the context string of the answer.

  const input = {
    queries: ['I feel depressed'],
    responses: [
      'I feel sad',
      'I feel happy',
    ]
  };
  var scores = [];
  const embeddings = model.embed(input);
  /*
    * The output of the embed method is an object with two keys:
    * {
    *   queryEmbedding: tf.Tensor;
    *   responseEmbedding: tf.Tensor;
    * }
    * queryEmbedding is a tensor containing embeddings for all queries.
    * responseEmbedding is a tensor containing embeddings for all answers.
    * You can call `arraySync()` to retrieve the values of the tensor.
    * In this example, embed_query[0] is the embedding for the query
    * 'How are you feeling today?'
    * And embed_responses[0] is the embedding for the answer
    * 'I\'m not feeling very well.'
    */
  scores = tf.matMul(embeddings['queryEmbedding'],
      embeddings['responseEmbedding'], false, true).dataSync();
  console.log(scores);
});

</script>

</body>
</html>

```
