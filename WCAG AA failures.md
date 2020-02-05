# WCAG quick reference AA failures

## Principle 1 – Perceivable

### Guideline 1.2 – Time-based Media

- 1.2.4 Captions (Live)
    - Captions are provided for all live audio content in synchronized media.        - 
- 1.2.5 Audio Description (Prerecorded)
    - Audio description is provided for all prerecorded video content in synchronized media.

### Guideline 1.3 – Adaptable

- 1.3.4 Orientation (Added in 2.1)
    - F97: Failure due to locking the orientation to landscape or portrait view 
- 1.3.5 Identify Input Purpose (Added in 2.1)
    - The purpose of each input field collecting information about the user can be programmatically determined. form input collecting information about the user. More than using the right `type` use e.g. `autocomplete=“given-name”`. See https://www.w3.org/TR/WCAG21/#input-purposes for list.

### Guideline 1.4 – Distinguishable.

- 1.4.3 Contrast (Minimum). The visual presentation of text and images of text has a contrast ratio of at least 4.5:1, except for Large Text, Logotypes.
    - F24: Failure of Success Criterion 1.4.3, 1.4.6 and 1.4.8 due to specifying foreground colors without specifying background colors or vice versa
    - F83: Failure of Success Criterion 1.4.3 and 1.4.6 due to using background images that do not provide sufficient contrast with foreground text (or images of text)
- 1.4.4 Resize text. Text can be resized without assistive technology up to 200 percent without loss of content or functionality.
    - F69: Failure of Success Criterion 1.4.4 when resizing visually rendered text up to 200 percent causes the text, image or controls to be clipped, truncated or obscured
    - F80: Failure of Success Criterion 1.4.4 when text-based form controls do not resize when visually rendered text is resized up to 200%
    - F94: Failure of Success Criterion 1.4.4 due to text sized in viewport units 
- 1.4.5 Images of Text. If the technologies being used can achieve the visual presentation, text is used to convey information rather than images of text
- 1.4.10 Reflow (Added in 2.1). Content can be presented without loss of information or functionality, and without requiring scrolling in two dimensions for: Vertical scrolling content at a width equivalent to 320 CSS pixels; Horizontal scrolling content at a height equivalent to 256 CSS pixels.
    - @@ Using fixed sized containers and fixed position content (CSS)
@@ (HTML) Using preformatted text or excluding preformatting text as an exception to no two dimensional scrolling.
    - F102: Failure of Success Criterion 1.4.10 due to content disappearing and not being available when content has reflowed
    - Use responsive web design!
- 1.4.11 Non-text Contrast (Added in 2.1). The visual presentation of the following have a contrast ratio of at least 3:1 against adjacent color(s).
    - F78: Failure of Success Criterion 2.4.7 due to styling element outlines and borders in a way that removes or renders non-visible the visual focus indicator 
- 1.4.12 Text Spacing (Added in 2.1). no loss of content or functionality occurs by setting all of the following and by changing no other style property: Line height (line spacing) to at least 1.5 times the font size; Spacing following paragraphs to at least 2 times the font size; Letter spacing (tracking) to at least 0.12 times the font size; Word spacing to at least 0.16 times the font size.
- 1.4.13 Content on Hover or Focus (Added in 2.1)
    - F95: Failure of Success Criterion 1.4.13 due to content shown on hover not being hoverable
    - @@ Failure to make content dismissable without moving pointer hover or keyboard focus
    - @@ Failure to meet by content on hover or focus not remaining visible until dismissed or invalid

## Principle 2 – Operable

### Guideline 2.4 – Navigable

- 2.4.5 Multiple Ways. Except where the Web Page is the result of, or a step in, a process.
    - Site map or search, `link rel`s
- 2.4.6 Headings and Labels. Headings and labels describe topic or purpose.
- 2.4.7 Focus Visible. Any keyboard operable user interface has a mode of operation where the keyboard focus indicator is visible.
    - F55: Failure of Success Criteria 2.1.1, 2.4.7, and 3.2.1 due to using script to remove focus when focus is received
    - F78: Failure of Success Criterion 2.4.7 due to styling element outlines and borders in a way that removes or renders non-visible the visual focus indicator 

## Principle 3 – Understandable

### Guideline 3.1 – Readable

- 3.1.2 Language of Parts. The human language of each passage or phrase in the content can be programmatically determined

### Guideline 3.2 – Predictable

- 3.2.3 Consistent Navigation. Unless a change is initiated by the user.
    - F66: Failure of Success Criterion 3.2.3 due to presenting navigation links in a different relative order on different pages 
- 3.2.4 Consistent Identification
    - F31: Failure of Success Criterion 3.2.4 due to using two different labels for the same function on different Web pages within a set of Web pages 
    
### Guideline 3.3 – Input Assistance

- 3.3.3 Error Suggestion. Unless it would jeopardize the security or purpose of the content.
    - Use client-side validation.
    - Use a `role="alertdialog”`
- 3.3.4 Error Prevention (Legal, Financial, Data). at least one of the following is true: Reversible: Submissions are reversible; Checked: Data entered by the user is checked for input errors and the user is provided an opportunity to correct them; Confirmed: A mechanism is available for reviewing, confirming, and correcting information before finalizing the submission.

## Principle 4 – Robust

### Guideline 4.1 – Compatible

- 4.1.3 Status Messages (Added in 2.1). In content implemented using markup languages, status messages can be programmatically determined through role or properties such that they can be presented to the user by assistive technologies without receiving focus.
    - Use `role”status”`
    - Using role="alert" or aria-live="assertive" on content which is not important and time-sensitive (future link)
  - Using a visibilitychange event to hide or display a document without switching the document's live regions between active and inactive (future link)
