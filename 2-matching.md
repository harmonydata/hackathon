# Task 2: Improve the matching algorithm

Harmony often matches items that should not be matched, or vice versa, e.g.

*Feeling tired or having little energy?* was incorrectly matched to *Having upsetting dreams that replay part of the experience or are clearly related to the experience?*

We have a Github repo where we have experimented with this: https://github.com/harmonydata/matching 

So how can we improve the matching? 

* Probably the easiest way would be to switch this underlying model, rather than trying anything clever.
* Longer term an LLM could be fine-tuned but that needs lots of resources and lots of data!

We could

* try different LLMs from HuggingFace
* add integration to OpenAI or Vertex
* run Tensorflow JS model in the front end (https://github.com/tensorflow/tfjs-models Universal Sentence Encoder) 

Check the code samples here for data and examples: https://github.com/harmonydata/matching 

Check this blog post too: https://harmonydata.ac.uk/measuring-the-performance-of-nlp-algorithms/

## Data

We have been evaluating the matching using the manually created harmonisation tool by McElroy et al:

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
