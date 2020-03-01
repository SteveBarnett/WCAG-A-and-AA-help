# WCAG A and AA failures with SC

- 1.1.1 Non-text Content
    - Using CSS to include images that convey important information
    - Having a text alternative that does not include information that is conveyed by color differences in the image
    - Updating text alternatives when changes to non-text content occur
    - Using text alternatives that are not alternatives (e.g., filenames or placeholder text)
    - Not marking up decorative images in HTML in a way that allows assistive technology to ignore them
    - Providing a text alternative that is not null (e.g., alt="spacer" or alt="image") for images that should be ignored by assistive technology
    - Omitting the alt attribute or text alternative on img elements, area elements, and input elements of type "image"
    - Providing long descriptions for non-text content that does not serve the same purpose or does not present the same information
    - Using text look-alikes to represent text without providing a text alternative
    - Using ASCII art without providing a text alternative
- 1.3.1 Info and Relationships
    - Using changes in text presentation to convey information without using the appropriate markup or text
    - Using white space characters to create multiple columns in plain text content
    - Using white space characters to format tables in plain text content
    - Using structural markup in a way that does not represent relationships in the content
    - Using th elements, layout tables
    - Using the pre element to markup tabular information
    - Inserting non-decorative content by using :before and :after pseudo-elements and the 'content' property in CSS
    - Incorrectly associating table headers and content via the headers and id attributes
    - Not correctly marking up table headers
    - Use of role presentation on content which conveys semantic information
- 1.3.2 Meaningful Sequence
    - Using white space characters to format tables in plain text content
    - Using white space characters to create multiple columns in plain text content
    - Using white space characters to control spacing within a word
    - Using an HTML layout table that does not make sense when linearized
    - Changing the meaning of content by positioning information with CSS
- 1.3.3 Sensory Characteristics
    - Identifying content only by its shape or location
    - Using a graphical symbol alone to convey information
- 1.3.4 Orientation (AA)
    - Locking the orientation to landscape or portrait view
- 1.3.5 Identify Input Purpose (Added in 2.1)
    - The purpose of each input field collecting information about the user can not be programmatically determined (does not use autocomplete)
- 1.4.1 Use of Color
    - Having a text alternative that does not include information that is conveyed by color differences in the image
    - Creating links that are not visually evident without color vision
    - Identifying required or error fields using color differences only
- 1.4.3 Contrast (Minimum)
    - Specifying foreground colors without specifying background colors or vice versa
    - Using background images that do not provide sufficient contrast with foreground text (or images of text)
- 1.4.4 Resize text
    - When resizing visually rendered text up to 200 percent causes the text, image or controls to be clipped, truncated or obscured
    - When text-based form controls do not resize when visually rendered text is resized up to 200%
    - Text sized in viewport units
- 1.4.5 Images of Text.
    - Images used where technologies being used could achieve the visual presentation using text
- 1.4.10 Reflow (AA)
    - Using fixed sized containers and fixed position content (CSS)
    - Using preformatted text or excluding preformatting text as an exception to no two dimensional scrolling
- 1.4.11 Non-text Contrast (Added in 2.1).
    - Styling element outlines and borders in a way that removes or renders non-visible the visual focus indicator
- 1.4.12 Text Spacing (Added in 2.1)
    - Loss of content or functionality occurs by setting all of the following and by changing no other style property: Line - height (line spacing) to at least 1.5 times the font size; Spacing following paragraphs to at least 2 times the font size; Letter spacing (tracking) to at least 0.12 times the font size; Word spacing to at least 0.16 times the font size.
- 1.4.13 Content on Hover or Focus (Added in 2.1)
    - Content shown on hover not being hoverable
    - Content not dismissable without moving pointer hover or keyboard focus
    - Content on hover or focus not remaining visible until dismissed or invalid
- 2.1.1 Keyboard. All functionality of the content is operable through a keyboard interface without requiring specific timings for individual keystrokes, except where the underlying function requires input that depends on the path of the user's movement and not just the endpoints.
    - Using only pointing-device-specific event handlers (including gesture) for a function
    - Using script to remove focus when focus is received
    - Emulating links incorrectly
- 2.1.2 No Keyboard Trap
    - Combining multiple content formats in a way that traps users inside one format type
- 2.1.4 Character Key Shortcuts (A)
    - includes single-key shortcuts that can't be turned off or remapped
- 2.2.1 Timing Adjustable
    - Using meta redirect with a time limit
    - Using meta refresh to reload the page
    - Using server-side techniques to automatically redirect pages after a time-out
- 2.2.2 Pause, Stop, Hide
    - Including scrolling content where movement is not essential to the activity without also including a mechanism to pause and restart the content
    - Using the blink element
    - Using text-decoration:blink without a mechanism to stop it in less than five seconds
    - A script that causes a blink effect without a mechanism to stop the blinking at 5 seconds or less
    - An object or applet, such as Java or Flash, for more than five seconds
- 2.3.1 Three Flashes or Below Threshold.
    - Contains content that flashes more than three times in any one second period
- 2.4.3 Focus Order
    - Using tabindex to create a tab order that does not preserve meaning and operability
    - Using dialogs or menus that are not adjacent to their trigger control in the sequential navigation order
- 2.4.4 Link Purpose (In Context)
    - Providing link context only in content that is not related to the link
    - Not providing an accessible name for an image which is the only content in a link
- 2.4.5 Multiple Ways. Except where the Web Page is the result of, or a step in, a process.
    - No site map, search, or link rels
- 2.4.6 Headings and Labels.
    - Headings and labels don't describe topic or purpose.
- 2.4.7 Focus Visible.
    - Using script to remove focus when focus is received
    - Styling element outlines and borders in a way that removes or renders non-visible the visual focus indicator
- 2.5.1 Pointer Gestures (A)
    - Multi-touch required for functionality
- 2.5.2 Pointer Cancellation (A)
    - Activating a button on initial touch location rather than the final touch location.
- 2.5.3 Label in Name (A)
    - Accessible name not containing the visible label text
    - Accessible name contains the visible label text, but the words of the visible label are not in the same order as they are in the visible label text
    - Accessible name contains the visible label text, but one or more other words are interspersed in the label
- 2.5.4 Motion Actuation (A)
    - Devicemotion events required for functionality
    - Unable to disable motion actuation
    - Disrupting or disabling system level features which allow the user to disable motion actuation
- 3.2 Labels or Instructions
    - Visually formatting a set of phone number fields but not including a text label.
- 4.1.1 Parsing
    - Incorrect use of start and end tags or attribute markup
    - Duplicate values of type ID
- 4.1.2 Name, Role, Value
    - Using script to make div or span a user interface control in HTML without providing a role for the control
    - Implementing custom controls that do not use an accessibility API for the technology, or do so incompletely
    - Not updating text alternatives when changes to non-text content occur
    - User interface control not having a programmatically determined name
    - Focus state of a user interface component not being programmatically determinable or no notification of change of focus state available
    - Not providing names for each part of a multi-part form field, such as a US telephone number
    - Not providing an accessible name for an image which is the only content in a link
- 4.1.3 Status Messages (AA)
    - Using role="alert" or aria-live="assertive" on content which is not important and time-sensitive
    - Using a visibilitychange event to hide or display a document without switching the document's live regions between active and inactive

---

Excluded:

- 1.2.1 Audio-only and Video-only (Prerecorded).
- 1.2.2 Captions (Prerecorded)
- 1.4.2 Audio Control