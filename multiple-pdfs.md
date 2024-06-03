# Harmony Matching Design Documentation
- Harmony competition: 03/06/2024
- Team name: Anomalies

## Problem
Harmony only harmonizes between 2 PDFs (of questionnaires/surveys), but we are looking into the possibility to expand this and think about how we would design how this would look like for 3 pages (and hopefully more in the future).

In order to make finding similarities between 3 PDFs, we considered the approach of sorting these matches using 1 core PDF which is compared to the other 2 PDFs. For example, if we were to have 3 PDFs (labelled A, B and C respectively), we would be using A as the core PDF and finding similarities in B and C that correlate to A. Which would translate to something like this: ![image](https://github.com/nlutala/hackathon/assets/87072306/847ae79f-bc0d-4109-88a3-3861c93921ee)

rather than this: ![image](https://github.com/nlutala/hackathon/assets/87072306/a0829795-ac31-441f-81a5-50a872589c74)
 
Using the current design of the website (see visual below), here are our thoughts:

![image](https://github.com/nlutala/hackathon/assets/87072306/d5ed60c6-8e45-4dce-8610-78eb4b18c17a)

### Harmony Filters
![image](https://github.com/nlutala/hackathon/assets/87072306/f7f7aba3-2885-42eb-9c2d-afbfeec4a619)

With the design above, we thought we could add more filters such as:
- Sorting by the study (or PDF)
- Search (same functionality)
- Other (search for other related topics around that word)

We believe that the "Show within-instrument matches" could be reworded in a way that is more understandable to the lay-user of the web application.

We also believe that the other functionalities provided by this widget is useful and should remain the same.

### Displaying Similarities on Harmony
![image](https://github.com/nlutala/hackathon/assets/87072306/1d62d239-87a4-4668-a80f-df07bc8863da)

Concerning the display of similar questions/statements across the PDFS ...
