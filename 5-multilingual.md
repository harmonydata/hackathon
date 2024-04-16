# Make Harmony multilingual

We focused on English and Portuguese for the development of Harmony.

For negation, Harmony currently identifies antonyms via a set of handwritten rules - inserting “not” (English) or “não” (Portuguese), etc. Can we improve this? Add more languages? https://github.com/harmonydata/harmony/blob/main/src/harmony/matching/negator.py 

Can we use different multingual LLMs such as the Shona sentence transformer [xlm-roberta-base-finetuned-shona](https://huggingface.co/Davlan/xlm-roberta-base-finetuned-shona) to add support for more languages?
