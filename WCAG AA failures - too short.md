# WCAG quick reference AA failures

- Captions or audio description are not provided for all content.
- Screen orientation is locked or viewport units are used to size text.
- `autocomplete` is not used for common fields. See https://www.w3.org/TR/WCAG21/#input-purposes.
- Contrast ratio is less than 4.5:1 (including `background-image`s), except for Large Text, Logotypes.
- Foreground colour is specified without background colour or vice versa.
- Images of text are used instead of text.
- Fixed-width containers and fixed position content are used.
- Increasing text size and spacing or viewing on a 256 x 320 screen loses content, loses functionality, or requires scrolling in two dimensions.
- Content shown on hover or focus doesn't stay until dismissed.
- Focus indicator is not visible or is removed by JS.
- `lang` is not set on `html`
- Navigation or labels for controls vary across pages.
- Using role="alert" or aria-live="assertive" on content which is not important and time-sensitive 
