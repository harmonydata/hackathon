# Harmony Matching Design Documentation
- Harmony competition: 03/06/2024
- Team name: Anomalies
- Team members: Shafna AbdulMajeed (https://www.linkedin.com/in/shafna-abdulmajeed-1790ba141/), Suqin Chua (https://www.linkedin.com/in/chuasuqin/), Nathan Lutala (https://www.linkedin.com/in/nathanlutala/)
- Compiled by Nathan Lutala on 03/06/2024; **Revised** by Shafna AbdulMajeed on 07/06/2024 (Revision 1).

## Problem
The Harmony tool harmonizes 2 or more data sets (i.e. studies/questionnaires/surveys) to find data matches, allowing researchers to collate similar questions across studies (in order to help collate similar data). At present the tool shows a 1:1 match which is not a big issue when 2 studies are being harmonized. However when 3 or more studies are being harmonized, 1:1 matching limits a researcher's speed and efficiency in quickly comprehending which questions match up across studies because the researcher has to manually match questions to questions.

We are looking at how best the dashboard could be represented to improve comprehension and lower cognitive load when 3 (or more) studies are being harmonized. Please scroll to the end of this README file to view an image of our solution (see "Comprehending Harmony: The Complete Picture").

To make comprehension easier, we considered the approach of representing matches by maintaining one base study, and having the other studies correspond or match up to the base study. Instead of 1:1 matching, this would be 1:x matching. For example, if we were to have 3 studies (labelled A, B and C), we would be using A as the base study and finding data matches in Studies B and C that correlate to A. In a simple diagramatic format, it would look like this:

![image](https://github.com/nlutala/hackathon/assets/87072306/847ae79f-bc0d-4109-88a3-3861c93921ee)

rather than the present condition which is this: 

![image](https://github.com/nlutala/hackathon/assets/87072306/a0829795-ac31-441f-81a5-50a872589c74)

## Proposal
Our proposal involves suggestions that could integrate into the existing design of the tool (see image below), in the areas of (1) Information Presentation and Comprehension, (2) Error Prevention and Match Accuracy, (3) Information Retrieval with Sorting and Filtering functionalities, as discussed in detail below.

![image](https://github.com/nlutala/hackathon/assets/87072306/d5ed60c6-8e45-4dce-8610-78eb4b18c17a)

### 1. Sorting Data Matches by Base Study (Default Display)
Currently data matches are displayed as 1:1 matches in descending match-percentage order:

![image](https://github.com/nlutala/hackathon/assets/87072306/1d62d239-87a4-4668-a80f-df07bc8863da)

Our design proposes that **data matches should be displayed by Base Study**, where one study is main one and all matches from other studies are shown against it. When a user uploads the studies they want to harmonize, the **first study uploaded will be designated as the base** study by default, e.g. Study A. The user **can choose to switch the base study** to study B or C etc. if needed or preferred.

This can be **enabled via a drop-down menu of studies in the existing 'Options' menu** on the left-hand side of the screen. There will **also be the option to 'Clear Sort'** to show 1:1 matches only, as per the current design. While the default Base Study Display was preferred in the user testing, specific use cases highlighted the need for users to be able to switch back to 1:1 match view.

In addition, **a horizontal filter above the data matches on the right-hand side of the screen** will be present to remind users which study is the Base Study while they are perusing data matches. Should they wish to quickly change the Base Study, they can click through this filter too, or choose to 'Clear Sort'.

In this default view, matches will be displayed by Base Study Questions in **chronological** order. Every question within the Base Study will be listed as its **own widget** e.g. Study A - Question 1. To clarify further, if Study A is the Base Study and has 10 questions, then 10 widgets will be displayed in the order of Question 1 to 10.

**Within a particular widget** e.g. for Question 1, **data matches** from Studies B and C will be **listed underneath in descending match-percentage order**, i.e. highest percentages will be shown first.

**Only the top 5 matches will be shown in each widget, with a "read more" button** at the bottom to **allow the user to expand the widget and see more data matches**. For example, **10 matches can be shown with a scroll bar** appearing on the side to see up to a designated number of matches within the widget. This interaction when 'Read More' is clicked is **yet to be designed and tested.**

Currently only 100 matches are shown per harmonization but the user can export all matches via an Excel sheet to see this in detail. We propose to maintain this function for the time being even with the new display format. This **could also be tested with users to determine if this is sufficient or could be improved.**

Below is an image of the design we have come up with for the right-hand side of the screen:

![image](https://github.com/nlutala/hackathon/assets/87072306/14f74612-08b1-466a-bc9f-848d8458b654)


### 2. Error Prevention
Harmony currently struggles with errors in data matching. Users have been asked to flag errors, providing reasons so that this can be fed back into the system to improve its matching capability. However, this is not a perfect system yet and the task of error prevention is heavy on the user.

To support the user to flag mismatches easily, we propose a **'See Context' button next to every data match**.

**On click, a pop-up window** could appear on the screen, displaying **side-by-side the entire question around the match and perhaps the questions before and after**. This provides more context to a data match (see image below), and should the user suspect that the suggested match is a mismatch, they could quickly refer the context to check their suspicion.

They can then either **flag the match if it is a mismatch**, or the context has clarified their concern.

![image](https://github.com/nlutala/hackathon/assets/87072306/8d42db27-3154-4b00-8565-3c6470ca87a6)


### 3. Filters for Information Sorting and Retrieval
Currently, the Options Menu on the left-hand side of the screen has a simple design as below:

![image](https://github.com/nlutala/hackathon/assets/87072306/f7f7aba3-2885-42eb-9c2d-afbfeec4a619)

We support the existing functions (Match Threshold, Search, Show Within-Instrument Matches, Just Selected Matches, Export). However, we suggest 3 improvements:
- The 'Show Within-Instrument Matches' could be **reworded to 'Show Within-Study Matches'** to be better **understood by lay-users or users across different industries**. This however would need to be tested with researchers and other users to determine if this is in fact an issue.
- Match Threshold should have **a number box below the slider** at each end to allow a user to input a number should they have **accessibility** issues that prevent them from using a slider.
- The Search Bar text could be **altered to 'Search Keywords'** (see 3a below) and could prompt keywords for users to search when they begin typing into the Search Bar.

We propose additional filters to aid information sorting and retrieval:
- Correlation Filter (positive correlation, negative correlation and complementary correlation) (See 3b below)
- Sorting Data Matches by Base Study (already explained above in Point 1)

#### 3a. Search Keywords
It is likely that users would already be searching for keywords that are displayed at the top of screen above the data matches, which are keywords or topics extracted from uploaded studies. To make the experience more intuitive, the Search Bar should **provide keyword prompts in response to the user typing**, thus making search **faster**.

Should the user write an entirely different word or phrase, they would **still be able to search their specific input**, maintaining original and **flexible** functionality.

#### 3b. Correlation Filter
We propose this additional filter to help users sort or filter matches to view only:
- Positive Correlations: shows a positive "similarity" score between a statement in the Base Study and same or similar statements in the corresponding studies.
- Negative Correlations: shows a negative "similarity" score between a statements in the Base Study and an opposite statement in the corresponding studies (linguistic antonymns and negations).
- Complementary Correlation: shows a low "similarity" score of the statements that are not similar or opposite, but where there may be an unexpected or unobvious similarity in a particular domain.

##### 3b.i. Positive Correlations (Same or Very Similar Statements)
This is similar to the functionality Harmony has already (the positive similarity scores). To view only these matches, the user could adjust the setting in the Correlation filter to "Positive".

##### 3b.ii. Negative Correlations (Opposite Statements)
This is similar to the functionality Harmony has already (the negative similarity scores). To view only these matches, the user could adjust the setting in the Correlation filter to "Negative".

##### 3b.iii. Complementary Correlations (Seemingly Low-Percentage Data Matches)
To support Error Prevention and aid better matching, we proposed this feature as a result of conversations with researchers at the Hackathon.

In the case where data matches have low similarity scores but are actually a match, e.g. a question asking about poor hygiene and a question asking about poor sleep could both be, by wider context, alluding to depression systems but because there is no obvious linguistic overlap, this would be a low or non-match. With the use of AI and algorithmic training by professionals in spcific domains that Harmony caters to, the system could be trained to suggested 'Complementary Matches' that are on the surface a low match. When the system does this, the reason for a complementary match should be highlighted to the user, e.g. via the 'See Context' pop-up. If it is not a match, the users should be able to report or flag it as not match to improve the system over time (see below). This suggestion has **not yet been designed in depth or tested.**

![image](https://github.com/nlutala/hackathon/assets/87072306/a4563d27-abf3-47b3-b151-a9a3a1c3bfd2)

We also thought it would be useful to utilize Harmony's ability to extract topics from uploaded studies as demonstrated below:

![image](https://github.com/nlutala/hackathon/assets/87072306/64ea73c4-0e26-4ea8-8851-7adb45e177ee)

To create a dropdown list to further filter 'Complementary Matches' based on these keywords/topics (see image below). However, please note the image below may need to be better articulated as **this functionality has not been deeply designed yet.**

![image](https://github.com/nlutala/hackathon/assets/87072306/9aca41c1-354b-46c2-8fbc-b68779c18004)

#### Filter Conclusion
**In conclusion with regards to the filters, the design proposal for the widget would be as follows (specifying instructions for order and functionalities) and image is shown below:**
**- Match Threshold**
**- Sort by Study. UX Copy to indicate 'Sorted by Study (A)' to show default setting. Drop-down menu to allow users to change base studies or select 'No Base Study'**
**- Seach Keywords**
**- Correlation Filter. When a filter is chosen, UX Copy to indicate chosen Correlation e.g. Positive Correlations Only. Accessed via a Drop-down menu indicating 'Positive Correlations, Negative Correlations, Complementary Correlations, No Correlations'**
**- 'Show Within-Study Matches'**
**- Just Selected Matches**
**- Export**

![image](https://github.com/nlutala/hackathon/assets/87072306/e5b9d8c3-4f2c-4c50-a06a-2d01e3d4a894)

## Conclusion: Comprehending Harmony
Here is our team's final proposal for Harmony 2.0. We hope that with this design, we could improve the comprehension of data matches when harmonizing studies, improve error prevention and match accuracy, and improve researcher speed and efficiency.

![image](https://github.com/nlutala/hackathon/assets/87072306/de29d863-e978-4e57-b53d-a9385a559cff)

## Limitations and Further Exploration
Limitations include:
- Limited and biased sample size. More testing with psychologists and researchers to gain their feedback on these design changes would provide a better understanding of its utility (especially those not affiliated with Harmony and have not used an AI tool to harmonise data before).
- Due to the new design, there could potentially be a lot of information shown on a page, meaning that users would have to scroll on the page more than necessary. How this is limited needs to be well-considered. In point 1 of this proposal, this is briefly touched on.

Further exploration would be needed for:
- Mobile Optimization
- Considering further filters that users may require, e.g. sorting  by recency/date, sorting by region etc.
