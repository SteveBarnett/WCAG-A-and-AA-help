# WCAG quick reference A failures

## Principle 1 – Perceivable

### Guideline 1.1 – Text Alternatives

- 1.1.1 Non-text Content
    - F3: Failure of Success Criterion 1.1.1 due to using CSS to include images that convey important information
    - F13: Failure of Success Criterion 1.1.1 and 1.4.1 due to having a text alternative that does not include information that is conveyed by color differences in the image
    - F20: Failure of Success Criterion 1.1.1 and 4.1.2 due to not updating text alternatives when changes to non-text content occur
    - F30: Failure of Success Criterion 1.1.1 and 1.2.1 due to using text alternatives that are not alternatives (e.g., filenames or placeholder text)
    - F38: Failure of Success Criterion 1.1.1 due to not marking up decorative images in HTML in a way that allows assistive technology to ignore them
    - F39: Failure of Success Criterion 1.1.1 due to providing a text alternative that is not null (e.g., alt="spacer" or alt="image") for images that should be ignored by assistive technology
    - F65: Failure of Success Criterion 1.1.1 due to omitting the alt attribute or text alternative on img elements, area elements, and input elements of type "image"
    - F67: Failure of Success Criterion 1.1.1 and 1.2.1 due to providing long descriptions for non-text content that does not serve the same purpose or does not present the same information
    - F71: Failure of Success Criterion 1.1.1 due to using text look-alikes to represent text without providing a text alternative
    - F72: Failure of Success Criterion 1.1.1 due to using ASCII art without providing a text alternative  

### Guideline 1.2 – Time-based Media

- 1.2.1 Audio-only and Video-only (Prerecorded). An alternative is provided that presents equivalent information.
    - F30: Failure of Success Criterion 1.1.1 and 1.2.1 due to using text alternatives that are not alternatives (e.g., filenames or placeholder text)
    - F67: Failure of Success Criterion 1.1.1 and 1.2.1 due to providing long descriptions for non-text content that does not serve the same purpose or does not present the same information 
- 1.2.2 Captions (Prerecorded)
    - F8: Failure of Success Criterion 1.2.2 due to captions omitting some dialogue or important sound effects
    - F75: Failure of Success Criterion 1.2.2 by providing synchronized media without captions when the synchronized media presents more information than is presented on the page
    - F74: Failure of Success Criterion 1.2.2 and 1.2.8 due to not labeling a synchronized media alternative to text as an alternative 
- 1.2.3 Audio Description or Media Alternative (Prerecorded)
- 1.2.4 Captions (Live)
    - Captions are provided for all live audio content in synchronized media.        - 
- 1.2.5 Audio Description (Prerecorded)
    - Audio description is provided for all prerecorded video content in synchronized media.

### Guideline 1.3 – Adaptable

- 1.3.1 Info and Relationships. Information, structure, and relationships conveyed through presentation can be programmatically determined or are available in text.
    - F2: Failure of Success Criterion 1.3.1 due to using changes in text presentation to convey information without using the appropriate markup or text
    - F33: Failure of Success Criterion 1.3.1 and 1.3.2 due to using white space characters to create multiple columns in plain text content
    - F34: Failure of Success Criterion 1.3.1 and 1.3.2 due to using white space characters to format tables in plain text content
    - F42: Failure of Success Criteria 1.3.1, 2.1.1, 2.1.3, or 4.1.2 when emulating links
    - F43: Failure of Success Criterion 1.3.1 due to using structural markup in a way that does not represent relationships in the content
    - F46: Failure of Success Criterion 1.3.1 due to using th elements, layout tables
    - F48: Failure of Success Criterion 1.3.1 due to using the pre element to markup tabular information
    - F87: Failure of Success Criterion 1.3.1 due to inserting non-decorative content by using :before and :after pseudo-elements and the 'content' property in CSS
    - F90: Failure of Success Criterion 1.3.1 for incorrectly associating table headers and content via the headers and id attributes
    - F91: Failure of Success Criterion 1.3.1 for not correctly marking up table headers
    - F92: Failure of Success Criterion 1.3.1 due to the use of role presentation on content which conveys semantic information 
- 1.3.2 Meaningful Sequence
    - F34: Failure of Success Criterion 1.3.1 and 1.3.2 due to using white space characters to format tables in plain text content
    - F33: Failure of Success Criterion 1.3.1 and 1.3.2 due to using white space characters to create multiple columns in plain text content
    - F32: Failure of Success Criterion 1.3.2 due to using white space characters to control spacing within a word
    - F49: Failure of Success Criterion 1.3.2 due to using an HTML layout table that does not make sense when linearized
    - F1: Failure of Success Criterion 1.3.2 due to changing the meaning of content by positioning information with CSS 
- 1.3.3 Sensory Characteristics
    - F14: Failure of Success Criterion 1.3.3 due to identifying content only by its shape or location
    - F26: Failure of Success Criterion 1.3.3 due to using a graphical symbol alone to convey information 
- 1.3.4 Orientation (Added in 2.1)
    - F97: Failure due to locking the orientation to landscape or portrait view 
- 1.3.5 Identify Input Purpose (Added in 2.1)
    - The purpose of each input field collecting information about the user can be programmatically determined. form input collecting information about the user. More than using the right `type` use e.g. `autocomplete=“given-name”`. See https://www.w3.org/TR/WCAG21/#input-purposes for list.

### Guideline 1.4 – Distinguishable

- 1.4.1 Use of Color. Color is not used as the only visual means of conveying information, indicating an action, prompting a response, or distinguishing a visual element.
    - F13: Failure of Success Criterion 1.1.1 and 1.4.1 due to having a text alternative that does not include information that is conveyed by color differences in the image
    - F73: Failure of Success Criterion 1.4.1 due to creating links that are not visually evident without color vision
    - F81: Failure of Success Criterion 1.4.1 due to identifying required or error fields using color differences only 
- 1.4.2 Audio Control
    - F23: Failure of 1.4.2 due to playing a sound longer than 3 seconds where there is no mechanism to turn it off
    - F93: Failure of Success Criterion 1.4.2 for absence of a way to pause or stop an HTML5 media element that autoplays 
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

### Guideline 2.1 – Keyboard Accessible

- 2.1.1 Keyboard.  All functionality of the content is operable through a keyboard interface without requiring specific timings for individual keystrokes, except where the underlying function requires input that depends on the path of the user's movement and not just the endpoints.
    - F54: Failure of Success Criterion 2.1.1 due to using only pointing-device-specific event handlers (including gesture) for a function
    - F55: Failure of Success Criteria 2.1.1, 2.4.7, and 3.2.1 due to using script to remove focus when focus is received
    - F42: Failure of Success Criteria 1.3.1, 2.1.1, 2.1.3, or 4.1.2 when emulating links 
- 2.1.2 No Keyboard Trap
    - F10: Failure of Success Criterion 2.1.2 and Conformance Requirement 5 due to combining multiple content formats in a way that traps users inside one format type 
- 2.1.4 Character Key Shortcuts. at least one of the following is true: turn off, remap, active only on focus.
    - Failure of Success Criteria 2.1.4 due to a webpage or web app that includes single-key shortcuts not including a control that allows users to turn the shortcuts off or a control that allows users to change the shortcuts to key combinations that include keys that are not upper or lower-case letters, punctuation, number, or symbol characters.

### Guideline 2.2 – Enough Time

- 2.2.1 Timing Adjustable. at least one of the following is true: turn off, adjust, extend.
    - F40: Failure of Success Criterion 2.2.1 and 2.2.4 due to using meta redirect with a time limit
    - F41: Failure of Success Criterion 2.2.1, 2.2.4, and 3.2.5 due to using meta refresh to reload the page
    - F58: Failure of Success Criterion 2.2.1 due to using server-side techniques to automatically redirect pages after a time-out 
- 2.2.2 Pause, Stop, Hide. For moving, blinking, scrolling, or auto-updating information, all of the following are true: Moving, blinking, scrolling (lasts more than five seconds); auto-updating - can be paused, stopped, hidden.
    - F16: Failure of Success Criterion 2.2.2 due to including scrolling content where movement is not essential to the activity without also including a mechanism to pause and restart the content
    - F47: Failure of Success Criterion 2.2.2 due to using the blink element
    - F4: Failure of Success Criterion 2.2.2 due to using text-decoration:blink without a mechanism to stop it in less than five seconds
    - F50: Failure of Success Criterion 2.2.2 due to a script that causes a blink effect without a mechanism to stop the blinking at 5 seconds or less
    - F7: Failure of Success Criterion 2.2.2 due to an object or applet, such as Java or Flash, for more than five seconds 
    
### Guideline 2.3 – Seizures and Physical Reactions

- 2.3.1 Three Flashes or Below Threshold. Web pages do not contain anything that flashes more than three times in any one second period
    - G19: Ensuring that no component of the content flashes more than three times in any 1-second period
    - G176: Keeping the flashing area small enough
    - G15: Using a tool to ensure that content does not violate the general flash threshold or red flash threshold 
    
### Guideline 2.4 – Navigable

- 2.4.1 Bypass Blocks. skip links, landmarks, headings, 
- 2.4.2 Page Titled
- 2.4.3 Focus Order
    - F44: Failure of Success Criterion 2.4.3 due to using tabindex to create a tab order that does not preserve meaning and operability
    - F85: Failure of Success Criterion 2.4.3 due to using dialogs or menus that are not adjacent to their trigger control in the sequential navigation order 
- 2.4.4 Link Purpose (In Context)
    - F63: Failure of Success Criterion 2.4.4 due to providing link context only in content that is not related to the link
    - F89: Failure of Success Criteria 2.4.4, 2.4.9 and 4.1.2 due to not providing an accessible name for an image which is the only content in a link 
- 2.4.5 Multiple Ways. Except where the Web Page is the result of, or a step in, a process.
    - Site map or search, `link rel`s
- 2.4.6 Headings and Labels. Headings and labels describe topic or purpose.
- 2.4.7 Focus Visible. Any keyboard operable user interface has a mode of operation where the keyboard focus indicator is visible.
    - F55: Failure of Success Criteria 2.1.1, 2.4.7, and 3.2.1 due to using script to remove focus when focus is received
    - F78: Failure of Success Criterion 2.4.7 due to styling element outlines and borders in a way that removes or renders non-visible the visual focus indicator 

### Guideline 2.5 – Input Modalities

- 2.5.1 Pointer Gestures
    - @@ Functionality can be operated by pointer input but not with single-point activation alone
- 2.5.2 Pointer Cancellation
    - @@ Failure of SC 2.5.3 due to activating a button on initial touch location rather than the final touch location.
- 2.5.3 Label in Name
    - F96: Failure due to the accessible name not containing the visible label text
    - @@ Accessible name contains the visible label text, but the words of the visible label are not in the same order as they are in the visible label text
    - @@ Accessible name contains the visible label text, but one or more other words are interspersed in the label
- 2.5.4 Motion Actuation. Functionality that can be operated by device motion or user motion can also be operated by user interface components and responding to the motion can be disabled to prevent accidental actuation,

## Principle 3 – Understandable

### Guideline 3.1 – Readable

- 3.1.1 Language of Page
- 3.1.2 Language of Parts. The human language of each passage or phrase in the content can be programmatically determined

### Guideline 3.2 – Predictable

- 3.2.1 On Focus. When any user interface component receives focus, it does not initiate a change of context.
- 3.2.2 On Input
    - F36: Failure of Success Criterion 3.2.2 due to automatically submitting a form and given a value
    - F37: Failure of Success Criterion 3.2.2 due to launching a new window without prior warning when the selection of a radio button, check box or select list is changed
- 3.2.3 Consistent Navigation. Unless a change is initiated by the user.
    - F66: Failure of Success Criterion 3.2.3 due to presenting navigation links in a different relative order on different pages 
- 3.2.4 Consistent Identification
    - F31: Failure of Success Criterion 3.2.4 due to using two different labels for the same function on different Web pages within a set of Web pages

### Guideline 3.3 – Input Assistance

- 3.3.1 Error Identification
    - G83: Providing text descriptions to identify required fields that were not completed
    - ARIA21: Using Aria-Invalid to Indicate An Error Field
    - SCR18: Providing client-side validation and alert 
    - ARIA18: Using aria-alertdialog to Identify Errors
    - ARIA19: Using ARIA role=alert or Live Regions to Identify Errors
    - ARIA21: Using Aria-Invalid to Indicate An Error Field
    - G84: Providing a text description when the user provides information that is not in the list of allowed values
    - G85: Providing a text description when user input falls outside the required format or values
    - SCR18: Providing client-side validation and alert
    - SCR32: Providing client-side validation and adding error text via the DOM 
- 3.3.2 Labels or Instructions
    - F82: Failure of Success Criterion 3.3.2 by visually formatting a set of phone number fields but not including a text label. Use labels, fields & legend
    - ARIA1: Using the aria-describedby property to provide a descriptive label for user interface controls
    - ARIA9: Using aria-labelledby to concatenate a label from several text nodes 
- 3.3.3 Error Suggestion. Unless it would jeopardize the security or purpose of the content.
    - Use client-side validation.
    - Use a `role="alertdialog”`
- 3.3.4 Error Prevention (Legal, Financial, Data). at least one of the following is true: Reversible: Submissions are reversible; Checked: Data entered by the user is checked for input errors and the user is provided an opportunity to correct them; Confirmed: A mechanism is available for reviewing, confirming, and correcting information before finalizing the submission

## Principle 4 – Robust

### Guideline 4.1 – Compatible

- 4.1.1 Parsing
    - F70: Failure of Success Criterion 4.1.1 due to incorrect use of start and end tags or attribute markup
    - F77: Failure of Success Criterion 4.1.1 due to duplicate values of type ID 
- 4.1.2 Name, Role, Value
    - F59: Failure of Success Criterion 4.1.2 due to using script to make div or span a user interface control in HTML without providing a role for the control
    - F15: Failure of Success Criterion 4.1.2 due to implementing custom controls that do not use an accessibility API for the technology, or do so incompletely
    - F20: Failure of Success Criterion 1.1.1 and 4.1.2 due to not updating text alternatives when changes to non-text content occur
    - F68: Failure of Success Criterion 4.1.2 due to a user interface control not having a programmatically determined name
    - F79: Failure of Success Criterion 4.1.2 due to the focus state of a user interface component not being programmatically determinable or no notification of change of focus state available
    - F86: Failure of Success Criterion 4.1.2 due to not providing names for each part of a multi-part form field, such as a US telephone number
    - F89: Failure of Success Criteria 2.4.4, 2.4.9 and 4.1.2 due to not providing an accessible name for an image which is the only content in a link
- 4.1.3 Status Messages (Added in 2.1). In content implemented using markup languages, status messages can be programmatically determined through role or properties such that they can be presented to the user by assistive technologies without receiving focus.
    - Use `role”status”`
    - Using role="alert" or aria-live="assertive" on content which is not important and time-sensitive (future link)
  - Using a visibilitychange event to hide or display a document without switching the document's live regions between active and inactive (future link)
