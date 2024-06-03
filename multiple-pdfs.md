# Harmony Matching Design Documentation
- Harmony competition: 03/06/2024
- Team name: Anomalies

## Problem
Harmony only harmonizes between 2 PDFs (of questionnaires/surveys), but we are looking into the possibility to expand this and think about how we would design how this would look like for 3 pages (and hopefully more in the future). Please be sure to scroll to the end of this README file to view an image of our design for our solution to handling more than 2 PDFs at a time (see Summary).

In order to make finding similarities between 3 PDFs, we considered the approach of sorting these matches using 1 core PDF which is compared to the other 2 PDFs. For example, if we were to have 3 PDFs (labelled A, B and C respectively), we would be using A as the core PDF and finding similarities in B and C that correlate to A. Which would translate to something like this: 

![image](https://github.com/nlutala/hackathon/assets/87072306/847ae79f-bc0d-4109-88a3-3861c93921ee)

rather than this: 

![image](https://github.com/nlutala/hackathon/assets/87072306/a0829795-ac31-441f-81a5-50a872589c74)
 
Using the current design of the website (see visual below), here are our thoughts:

![image](https://github.com/nlutala/hackathon/assets/87072306/d5ed60c6-8e45-4dce-8610-78eb4b18c17a)

### Harmony Filters
![image](https://github.com/nlutala/hackathon/assets/87072306/f7f7aba3-2885-42eb-9c2d-afbfeec4a619)

With the design above, we thought we could add more filters such as:
- Sorting by the study (or PDF)
- Search keywords
- Correlation filter

We believe that the "Show within-instrument matches" could be reworded in a way that is more understandable to the lay-user of the web application.

We also believe that the other functionalities provided by this widget is useful and should remain the same.

Here is how we would imagine the new widget would look like:

![image](https://github.com/nlutala/hackathon/assets/87072306/e5b9d8c3-4f2c-4c50-a06a-2d01e3d4a894)


#### Sorting by the study (or PDF)
In this feature, the end user can choose the base PDF to compare the other PDFs to. We imagine that this would be a dropdown menu showing the PDFs the user has uploaded to harmony.

#### Search Keywords
In this filter, we imagine that the end user can start typing a word that they would like to look for in the matches and be able to see matches related to that word. 

#### Correlation Filter
This is a new feature with the following categories:
- Same: shows a similarity score between a statement in the core PDF and the similar statements in the other 2 PDFs
- Opposites: shows a "similarity" score of the statements opposite to the one in the core PDF in the other 2 PDFs
- Complementary: shows a "similarity" score of the statements that are not similar or opposite to the core PDF at first glance, but where there may be a similarity under a different lense. (linguistic antonymns and denials/negations)

### Displaying Similarities on Harmony
![image](https://github.com/nlutala/hackathon/assets/87072306/1d62d239-87a4-4668-a80f-df07bc8863da)

Concerning the display of similar questions/statements across the PDFS, we imagine that the user will be able to sort the matches at the PDF level.

In the image below, PDF A is taken as the core PDF for the other studies (B and C) to compare against. This is shown as its own widget with one statement/question from PDF A and a list of statements/questions from the PDFs B and C and it's similarity score.

Next to the statements/questions, there is a "see context" which we imagine would open a pop-up, displaying where in the PDF this statement appears so that the user is provided with more context and can be better informed about whether it is in fact similar to the statement from the core PDF (see image below).

![image](https://github.com/nlutala/hackathon/assets/87072306/8d42db27-3154-4b00-8565-3c6470ca87a6)

Under each widget, there is a "see more" button that allows the user to see the similarity scores for all the statements/questions found in PDF B and C that Harmony was able to identify as a match for the one statement/question in PDF A.

Below is an image of the overall design we have come up with (considering the right-hand side of the page at /app/#/model)

![image](https://github.com/nlutala/hackathon/assets/87072306/14f74612-08b1-466a-bc9f-848d8458b654)

#### Same
See section above

#### Opposites

#### Complementary

## Limitations
- Limited and biased sample size: we believe that more testing with psychologists and their viewpoints on this design would be beneficial (especially those not affiliated with Harmony and have not used an AI tool to harmonise data before).
- Due to the new design, there could potentially be a lot of information shown on a page, meaning that users would have to scroll on the page more than necessary.
- Consider how it looks and optimises on mobile
- Consider type of filters that users may require, e.g. sorting  by recency/date, sorting by region etc.

## Summary
Here is our team's diagram on the design of harmony if we could expand the functionality to handle more than 2 PDFs at a time

![image](https://github.com/nlutala/hackathon/assets/87072306/de29d863-e978-4e57-b53d-a9385a559cff)

