# WCAG A and AA failures - manual checks

(Things that won't get picked up by axe)

## Level A

- Any non-text content that changes without user interaction can't be turned off, adjusted, or extended (unless it's very short / small)
- Logical and standard order and behaviours aren't followed
- No helpful navigation exists: good page title, skip links, landmarks, or headings
- Some functionality is not available from a keyboard

## Level AA

- autocomplete is not used for common fields. See https://www.w3.org/TR/WCAG21/#input-purposes.
- Content shown on hover or focus doesn't stay until dismissed.
- Focus indicator is not visible or is removed by JS.
- Navigation or labels for controls vary across pages.
- Using role="alert" or aria-live="assertive" on content which is not important and time-sensitive
