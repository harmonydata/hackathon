# Task 7. Give a similarity function between questionnaires (the H-score!)

Eve Cheng has done some experiments with the Word Movers Distance algorithm which gives the distance between two sequences of sentence embeddings.

Can Harmony use this to say that the GAD-7 is e.g. 60% similar to the PHQ-9?

See Colab notebook:
https://github.com/harmonydata/experiments/blob/main/harmony_wmd_experiment.ipynb

We also have a demo of Harmony integrated with external data sources: https://harmonycataloguelookup.azurewebsites.net/

Source code is at: https://github.com/harmonydata/harmony_catalogue_lookup_dash

The use case would be:

```
as a research psychologist, I’ve got one small study here, one small study there. Individually they don’t give enough statistical power, but can they do it together? So can we combine Study A and Study B to get enough statistical power for my research question?
```
