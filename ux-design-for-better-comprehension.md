# Design Documentation: Improving Harmony's Dashboard for Better Comprehension and Efficiency
- Harmony Hackathon competition: 03/06/2024
- Team name: Anomalies
- Team members: Shafna AbdulMajeed (https://www.linkedin.com/in/shafna-abdulmajeed-1790ba141/), SuQin Chua (https://www.linkedin.com/in/chuasuqin/), Nathan Lutala (https://www.linkedin.com/in/nathanlutala/)
- Compiled by Nathan Lutala on 03/06/2024; **Revised** by Shafna AbdulMajeed on 07/06/2024 (Revision 1); **Revised** by SuQin Chua on 10/06/2024 (Revision 2);

## Context
The Harmony tool uses Natural Language Processing (NLP) for retrospective harmonisation of questionnaire items. It is currently capable of only harmonising two studies (i.e. questionnaires, surveys) to find matches using 1:1 comparison logic. The benefits of this tool allows researchers to collate similar questions across studies to help collate similar data. 

## Problem
Through conversations with Harmony team psychologists, we identified a user need for harmonising three or more sets of studies to optimise a researcher's (user's) speed and efficiency. Enabling greater comparison between different studies will allow researchers to quickly determine which questions align across studies and their respective similarity scores. The current 1:1 matching process, which still requires a degree of manual matching, limits their speed and efficiency.

In this investigation, we decided to look at how we can best visualise the Harmony dashboard to improve comprehension and lower cognitive load when three studies are harmonised. Please scroll to the end of this README file to view an image of our solution (see "Comprehending Harmony: The Complete Picture").

To make it easier for users to understand, we considered using the comparison logic of maintaining one base study as a reference point and have the other studies match up to the base study. So, instead of 1:1 matching, this would be 1:x matching. For example, if we were to have 3 studies (labelled A, B and C), we would be using A as the base study (reference point) and finding data matches in Studies B and C that correlate to A. In a simple diagramatic format, it would look like this:

![image](https://github.com/nlutala/hackathon/assets/87072306/847ae79f-bc0d-4109-88a3-3861c93921ee)

rather than the present condition which is this: 

![image](https://github.com/nlutala/hackathon/assets/87072306/a0829795-ac31-441f-81a5-50a872589c74)

## Proposal
Our proposal involves suggestions that could integrate into the existing design of the tool (see image below), in the areas of (1) Information Presentation and Comprehension, (2) Error Prevention and Match Accuracy, (3) Information Retrieval with Sorting and Filtering functionalities, as discussed in detail below.

![image](https://github.com/nlutala/hackathon/assets/87072306/d5ed60c6-8e45-4dce-8610-78eb4b18c17a)

### 1. Sorting Data Matches by Base Study (Default Display)
Currently data matches are displayed as 1:1 matches in descending similarity match-percentage order:

![image](https://github.com/nlutala/hackathon/assets/87072306/1d62d239-87a4-4668-a80f-df07bc8863da)

Our design proposes that **data matches should be displayed by Base Study**, where one study is the main reference point and all matches from other studies are shown and compared against it. When a user uploads the studies they want to harmonise, the **first study uploaded will be designated as the base** study by default. If the user wishes to switch out Study A to a different study as the Base, they **can then choose to switch the base study** to Study B or C etc. if needed or preferred.

This can be **enabled via a drop-down menu of studies in the existing 'Options' menu** on the left side of the screen. There will **also be the option to 'Clear Sort'** to show 1:1 matches, as per current design. In a quick preference test with users, the default Base Study Display was preferred. However, some users highlighted specific use cases and needs to be able to switch back to 1:1 match view for broader comparison.

To support ease of use, **a 'Study Key' filter above the data matches on the right-hand side of the screen** will remind users which study is currently the reference Base Study. Should they wish to quickly change this, they can quickly select the Study they want via radio buttons, or choose to 'Clear Sort'.

In this default view, matches will be displayed by Base Study Questions in **chronological** order. Every question within the Base Study will be listed as its **own widget** e.g. Study A - Question 1. To clarify further, if Study A is the Base Study and has 10 questions, then 10 widgets will be displayed in ascending order of Question 1 to 10.

**Within a particular widget** e.g. for Question 1, **data matches** from Studies B and C will be **listed underneath in descending match-percentage order**, i.e. highest percentages will be shown first.

**Only the top five matches will be shown in each widget, with a 'read more' CTA** at the bottom to **allow the user to expand the widget and view more data matches**. For example, **10 matches can be shown with a scroll bar** appearing on the side to see up to a designated number of matches within the widget. *This interaction with 'Read More' is yet to be designed and tested.*

Currently only 100 matches are shown per harmonisation but the user can export all matches via an Excel sheet to see this in detail. We propose to maintain this function for the time being even with the new display format. This **could also be tested with users to determine if this is sufficient or could be improved.**

Below is an image of the design we have come up with for the right-hand side of the screen:

![image](https://github.com/nlutala/hackathon/assets/87072306/14f74612-08b1-466a-bc9f-848d8458b654)


### 2. Error Prevention
Harmony is still training it's algorithms to provide matches more accurately. Currently, there is a function to allow for users to flag errors so it can be fed back into the system to improve its matching capability. However, this is not a perfect system yet and still requires a deal of manual error checking.

To support the user to identify errors in matches more easily, we propose a **'See Context' button next to every data match**.

**On click, a pop-up window** could appear on the screen, displaying **the two contexts which the texts are extracted from side-by-side**. This approach provides users with more context for each data match (see image below). If users suspect an inaccuracy in the suggested match, they can quickly refer to the context to verify their suspicion.

They can then either **flag the match if it is a mismatch**, or **see context** to clarify their concern.

![image](https://github.com/nlutala/hackathon/assets/87072306/8d42db27-3154-4b00-8565-3c6470ca87a6)


### 3. Filters for Information Sorting and Retrieval
Currently, the Options Menu on the left side of the screen has a simple design as below:

![image](https://github.com/nlutala/hackathon/assets/87072306/f7f7aba3-2885-42eb-9c2d-afbfeec4a619)

In addition to the existing functions: Match Threshold, Search, Show Within-Instrument Matches, Just Selected Matches, Export, we suggest three improvements:
- 'Show Within-Instrument Matches' could be **reworded to 'Show Within-Study Matches'** to **avoid jargon and allow easier understanding for a wider group of users**. *This has yet to be tested with potential users to determine if this is in fact an issue.*
- Match Threshold should have **a value input box below the slider** at each end to allow a user to specify a number for their required study. This also improves **accessibility** and can prevent errors or slips from using a slider.
- Consider adjusting the Search Bar text to **include 'Search Keywords'** (see 3a below) and prompt keywords for users to select when typing in the Search Bar.

We propose **two additional filters** to aid information sorting and retrieval:
- Correlation Filter (positive correlation, negative correlation and complementary correlation) (See 3b below)
- Sorting Data Matches by Base Study (explained above in Point 1)

#### 3a. Search Keywords
The Harmony tool generates a keyword cloud of themes when two studies are harmonised. It is likely that users would use the keywords generated in that section (above matches) in their searches. To make the experience more intuitive, the Search Bar should **provide keyword prompts in response to the user typing**, thus making search **faster**.

Should the user write an entirely different word or phrase, it is recommended that they could still be able to search for their specific input, **maintaining original and flexible functionality.**

#### 3b. Correlation Filter
We propose this additional filter to help users sort or filter matches to view only:
- Positive Correlations: shows a positive "similarity" score between a statement in the Base Study and same or similar statements in the corresponding studies.
- Negative Correlations: shows a negative "similarity" score between a statements in the Base Study and an opposite statement in the corresponding studies (linguistic antonymns and negations).
- Complementary Correlation: shows a low "similarity" score of the statements that are not similar or opposite, but where there may be an unexpected or unobvious similarity in a particular domain.

#### 3b.i. Positive Correlations (Same or Very Similar Statements)
This is similar to the functionality Harmony has already implemented (positive similarity scores). To view only these matches, the user could adjust the setting in the Correlation filter to "Positive".

#### 3b.ii. Negative Correlations (Opposite Statements)
This is similar to the functionality Harmony has already implemented (negative similarity scores). To view only these matches, the user could adjust the setting in the Correlation filter to "Negative".

#### 3b.iii. Complementary Correlations (Seemingly Low-Percentage Data Matches)
To support Error Prevention and aid better matching, we proposed this feature as a result of conversations with psychologists from Harmony at the Hackathon.

It is possible that the data matches could have low similarity scores but are actually related through other dimensions. For example, a question about poor hygiene and a question about poor sleep from another study could both allude to depression symptoms, but the lack of obvious linguistic overlap can result in a low or non-match percentage score.

With the use of AI and algorithmic training by professionals in specific domains that Harmony caters to, the system could be trained to suggest 'Complementary Matches'.

When the system makes a complementary match, the reason should be highlighted to the user through a 'See Context' pop-up (see Point 2). If the match is incorrect, users should be able to report or flag it to help improve the system over time (see below). *This suggestion has not yet been fully designed or tested.*

![image](https://github.com/nlutala/hackathon/assets/87072306/a4563d27-abf3-47b3-b151-a9a3a1c3bfd2)

We also thought it would be useful to utilise Harmony's ability to extract topics from uploaded studies as demonstrated below:

![image](https://github.com/nlutala/hackathon/assets/87072306/64ea73c4-0e26-4ea8-8851-7adb45e177ee)

To create a dropdown list to further filter 'Complementary Matches' based on these keywords/topics (see image below). However, please note the image below may need to be better articulated as *this functionality has not been deeply designed yet.*

![image](https://github.com/nlutala/hackathon/assets/87072306/9aca41c1-354b-46c2-8fbc-b68779c18004)

**In conclusion, our design proposal for the filter widgets would be as follows (specifying instructions for order and functionalities):**
- Match Threshold
- Sort by Study. UX Copy to indicate 'Sorted by Study (A)' to show default setting. Drop-down menu to allow users to change base studies or select 'No Base Study'
- Seach Keywords
- Correlation Filter. When a filter is chosen, UX Copy to indicate chosen Correlation e.g. Positive Correlations Only. Accessed via a Drop-down menu indicating 'Positive Correlations, Negative Correlations, Complementary Correlations, No Correlations'
- 'Show Within-Study Matches'
- Just Selected Matches
- Export

![image](https://github.com/nlutala/hackathon/assets/87072306/e5b9d8c3-4f2c-4c50-a06a-2d01e3d4a894)

## Conclusion: Comprehending Harmony
In conclusion, here is our team's final proposal for Harmony. With this design, we aim to enhance the understanding of data matches during study harmonization, prevent errors, increase match accuracy, and boost researcher speed and efficiency.

![image](https://github.com/nlutala/hackathon/assets/87072306/de29d863-e978-4e57-b53d-a9385a559cff)

## Limitations and Further Exploration
Given the constraints of the hackathon, the limitations include:
- Limited and biased sample size. More testing with psychologists and a wider group of researchers can provide more detailed feedback on these design changes and a better understanding of its utility, especially those who are not affiliated with Harmony and/or new to AI tools. It would also be beneficial to test this with users who are relatively new or juniors in the field. 
- As this is a new design, there is a potential for information overload to occur as this is a information-heavy product. More detail shown could lead to more users scrolling on the page than necessary. How this is limited needs to be well-considered. This has been briefly touched on in point 1 of this proposal.

**Further exploration would be needed for:**
- Mobile Optimisation
- Considering further filters that users may require, e.g. sorting  by recency or date, sorting by region etc.
