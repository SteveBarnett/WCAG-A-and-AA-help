# WCAG quick reference A failures

## Principle 1 – Perceivable

### Guideline 1.1 – Text Alternatives

- Missing or bad alt text.
- Meaningful images or colour use with no or bad text alternatives.
- Decorative images not marked as such.
- Using text as images, except logos.

### Guideline 1.2 – Time-based Media

- Prerecorded audio or video has no or bad (e.g. not equivalent, incomplete) text alternatives.

### Guideline 1.3 – Adaptable

- White space, `pre` element, or tables used for formatting or layout.
- Semantically incorrect markup used.
- Tables have invalid markup or don't make sense when linearised (i.e. in HTML source order).
- Meangingful content marked as decorative (e.g. `role="presentation"`)
- Using visual-only language ("the green circle to the left"), using symbols without a text equivalent.
- CSS positioning or `:before`/`:after` is used to mess with the meaning of the content


### Guideline 1.4 – Distinguishable

- Color is used as the only visual means of conveying information (such as state change or errors).
- Links don't look different without colour vision.
- Audio longer than 3 seconds, or anything autoplaying, can't be stopped.

## Principle 2 – Operable

### Guideline 2.1 – Keyboard Accessible

- Keyboard can't be used for sections of the UI because a pointer (mouse/trackpad) is required, focus is lost, the keyboard gets trapped, except where the function requires a pointer.
- Key shortcuts can't be turned off, remapped, or are always active.

### Guideline 2.2 – Enough Time

- Timing can't be turned off, adjusted, or extended, including `meta` `redirect`s and `refresh`es.
- Moving, blinking, scrolling lasts more than 5 seconds.
- Auto-updating information can't be paused, stopped, or hidden.
    
### Guideline 2.3 – Seizures and Physical Reactions

- Some elements flash more than 3 times a second, or are large.

### Guideline 2.4 – Navigable

- There are no skip links, landmarks, or headings.
- There's no good page title.
- The focus order doesn't preserve meaning.
- Trigger and target are not in sequential navigation order.
- Links (or images as links) don't make sense in context or have accessible names

### Guideline 2.5 – Input Modalities

- Some actions require multi-touch or device motion.
- Button event fire immediately on touch.
- Accessible names are different to visual names.

## Principle 3 – Understandable

### Guideline 3.1 – Readable

- 3.1.1 Language of Page

### Guideline 3.2 – Predictable

- Keyboard focus changes context.
- Forms auto-submit.
- Forms open new windows.

### Guideline 3.3 – Input Assistance

- (No documented Failures, but lots of Sufficient and Advisory Techniques)

## Principle 4 – Robust

### Guideline 4.1 – Compatible

- The HTML doesn't validate (e.g. missing start or end tags, bad attributes, duplicate IDs)
- Custom controls must have accessible Name, Role, Value, be focusable
