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

Check the code samples here for data and examples: https://github.com/harmonydata/matching 

Check this blog post too: https://harmonydata.ac.uk/measuring-the-performance-of-nlp-algorithms/

## Data

Tool by McElroy et al:

https://github.com/harmonydata/harmony_original/blob/main/data/Final%20harmonised%20item%20tool%20EM.xlsx

