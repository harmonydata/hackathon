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
- Compliance: Pass
#### 2.2 Time-based Media
Audio/Video should have captions and transcripts. Video content should have audio descriptions (AD)
- Compliance: Pass
- Comment: Captions are currently auto-generated and may show some inaccuracies. Consider uploading your own captions for any videos in the future.
#### 2.3 Adaptable
Content should be structured using proper headings h1 to h6. Landmarks should also be marked up correctly, e.g. header, nav, main, footer.
- Compliance: Fail
- Severity: Medium
- Comment: Consider providing headings on the right-hand side of the dashboard to inform users what the content is showing and what functionalities are available with appropriate markup.
#### 2.4 Distinguishable
Colour Contrast should be 4.5:1 for normal text, 3:1 for large text. Text should be able to be resized up to 200% without loss of content or functionality.
- Compliance: Fail
- Severity: Medium
- Comment:

### Operable
#### 3.1 Keyboard Accessible
Ensure all interactive elements (links, buttons, form controls) are keyboard accessible and focus indicators are visible.
- Compliance: Fail
- Severity: Medium
- Comment: Keyboard does not tab to My Harmony and Select All - which are key functionalities of the tool.
#### 3.2 Enough Time
Check for adjustable or extendable time limits.
- Compliance: Fail
- Severity: Medium
- Comment:
#### 3.3 Seizures and Physical Reactions
Ensure content does not contain flashes that could cause seizures (no more than 3 flashes per second).
- Compliance: Fail
- Severity: Medium
- Comment:
#### 3.4 Navigable
Navigation: Ensure navigation order is logical and consistent; include skip links. Ensure all pages have descriptive titles and every link text is descriptive and meaningful.
- Compliance: Fail
- Severity: Medium
- Comment:

### Understandable
#### 4.1 Readable
Ensure the language of the page is declared in the HTML and content that is readable and understandable for the intended audience.
- Compliance: Fail
- Severity: Medium
- Comment:
#### 4.2 Predictable
Ensure navigation and interactive elements are consistent throughout the site. Also ensure changes in context, e.g. opening in new window, are precitable and notified to the user.
- Compliance: Fail
- Severity: Medium
- Comment:
#### 4.3 Input Assistance
Ensure form elements have associated labels.Check for clear instructions and error messages, and suggestions for correction are provided.
- Compliance: Fail
- Severity: Medium
- Comment:

### Robust
#### 5.1 Compatible
Ensure compatibility with various assistive technologies like screen readers or voice recognition software. Also ensure HTML/CSS is valid and follows best practices.
- Compliance: Fail
- Severity: Medium
- Comment:
## Recommendations
Summary of Findings:

Areas of Improvement:

Immediate Actions:

Long-term Strategies:

#### Compliance Level
Overall Compliance Level Achieved:
