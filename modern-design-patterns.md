# WCAG A and AA failures with SC

Some common modern design patterns can cause WCAG Failures. Here are three that I've seen a few times:

- Removing underlines from links and the link colour not being contrast-y enough compared to the body text. This is [failure 73](https://www.w3.org/WAI/WCAG21/Techniques/failures/F73.html) of [1.4.1 Use of Color](https://www.w3.org/WAI/WCAG21/quickref/?currentsidebar=%23col_overview&techniques=sufficient%2Cadvisory&technologies=smil%2Cpdf%2Cflash%2Csl#use-of-color)
- Doing responsive typography by using viewport units. This is [Failure 94](https://www.w3.org/WAI/WCAG21/Techniques/failures/F94.html) under [1.4.4 Resize text](https://www.w3.org/WAI/WCAG21/quickref/?currentsidebar=%23col_overview&techniques=sufficient%2Cadvisory&technologies=smil%2Cpdf%2Cflash%2Csl#resize-text).
- Using fixed position content. This is a failure under [1.4.10 Reflow](https://www.w3.org/WAI/WCAG21/quickref/?currentsidebar=%23col_overview&techniques=sufficient%2Cadvisory&technologies=smil%2Cpdf%2Cflash%2Csl#reflow).

## List of some common Failures by Success Criteria

- 1.4.1 Use of Color
    - Creating links that are not visually evident without color vision
- 1.4.4 Resize text
    - Text sized in viewport units
- 1.4.10 Reflow
    - Using fixed sized containers and fixed position content (CSS)
