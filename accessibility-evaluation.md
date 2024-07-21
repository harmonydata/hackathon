# Accessibility documentation: Harmony tool
- Evaluation: July 2024
- Done by Suqin Chua (https://www.linkedin.com/in/chuasuqin/)

## What is web accessibility?
The Web Content Accessibility Guidelines (WCAG) are an internationally recognised set of recommendations for improving web accessibility, to ensure websites and apps are made accessible for everyone.

There are four design principles:
1. Perceivable
2. Operable
3. Understandable
4. Robust

There are 13 guidelines in WCAG 2.2. Each of these is broken down into specific requirements (or ‘success criteria’) that your service needs to meet. To ensure your design, code and content comply with WCAG, you should conduct regular accessibility testing with assitive technologies and meet a standard of Level AA (passing Level A too).

## General Information
Standards applied: WCAG 2.2

Tools used: Screen reader (Narrator, on Windows)

Pages Audited:
1. https://harmonydata.ac.uk/app/#/
2. https://harmonydata.ac.uk/app/#/model

## Accessibility audit
### Perceivable
#### 2.1 Text Alternatives
Images should have appropriate alt text; decorative images should have empty alt attributes.
Severity:

Compliance:

#### 2.2 Time-based Media
Audio/Video should have captions and transcripts. Video content should have audio descriptions (AD)
#### 2.3 Adaptable
Content should be structured using proper headings h1 to h6. Landmarks should also be marked up correctly, e.g. header, nav, main, footer.
#### 2.4 Distinguishable
Colour Contrast should be 4.5:1 for normal text, 3:1 for large text. Text should be able to be resized up to 200% without loss of content or functionality.

### Operable
#### Keyboard Accessible
Ensure all interactive elements (links, buttons, form controls) are keyboard accessible and focus indicators are visible.

Compliance: Fail

Severity: Medium

Comment: Keyboard does not tab to My Harmony and Select All - which are key functionalities of the tool.
#### Enough Time
Check for adjustable or extendable time limits.
#### Seizures and Physical Reactions
Ensure content does not contain flashes that could cause seizures (no more than 3 flashes per second).
#### Navigable
Navigation: Ensure navigation order is logical and consistent; include skip links. Ensure all pages have descriptive titles and every link text is descriptive and meaningful.

### Understandable
#### Readable
Language:
Ensure the language of the page is declared in the HTML.
Reading Level:
Check for content that is readable and understandable for the intended audience.
#### Predictable
Consistency:
Ensure navigation and interactive elements are consistent throughout the site.
Unexpected Changes:
Verify that changes in context (e.g., new pages opening) are predictable and notified.
#### Input Assistance
Forms:
Ensure form elements have associated labels.
Check for clear instructions and error messages.
Verify that input errors are identified and suggestions for correction are provided.
### Robust
#### Compatible
Assistive Technologies:
Verify that the website is compatible with various assistive technologies (e.g., screen readers, speech recognition software).
HTML Validation:
Ensure HTML/CSS is valid and follows best practices.

## Recommendations
Summary of Findings:

Areas of Improvement:

Immediate Actions:

Long-term Strategies:

#### Compliance Level
Overall Compliance Level Achieved:
