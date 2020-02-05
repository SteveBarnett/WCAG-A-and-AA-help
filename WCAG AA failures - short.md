# WCAG quick reference AA failures

## Principle 1 – Perceivable

### Guideline 1.2 – Time-based Media

- Captions are not provided for all live audio content.
- Audio description is not provided for all prerecorded video content.

### Guideline 1.3 – Adaptable

- Screen orientation is locked.
- `autocomplete` is not used for common fields. See https://www.w3.org/TR/WCAG21/#input-purposes.

### Guideline 1.4 – Distinguishable.

- Contrast ratio is less than 4.5:1 (including `background-image`s), except for Large Text, Logotypes.
- Foreground colour is specified without background colour or vice versa.
- Resizing text to 200% loses content, functionality, or clips, truncates, obscures, or loses content.
- Text is sized in viewport units.
- Images of text are used instead of text.
- Viewing on 256 x 320 screen requires scrolling in two dimensions.
- Fixed-width containers and fixed position content are used.
- Focus styles aren't visible.
- Loss of content or functionality occurs by setting : `line-height` 1.5 times font size; `margin` following paragraphs 2 times the font size; `letter-spaacing` 0.12 times the font size; `word-spacing`0.16.
- Content shown on hover not being hoverable, dismissable without moving pointer hover or keyboard focus
- Content on hover or focus doesn't remain visible until dismissed or invalid

## Principle 2 – Operable

### Guideline 2.4 – Navigable

- Focus indicator is not visible, is removed by JS.

## Principle 3 – Understandable

### Guideline 3.1 – Readable

- `lang` is not set on `html`

### Guideline 3.2 – Predictable

- Navigation varies across pages
- Labels for the same control vary across pages

## Principle 4 – Robust

### Guideline 4.1 – Compatible

- Using role="alert" or aria-live="assertive" on content which is not important and time-sensitive 
