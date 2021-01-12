# Tip47: Distinguish Between Real Line and Display Lines

A single line in the file may be represented by multiple lines on the display.

**Real Lines**: begin with a number, may span one or more display lines.
**Display Lines**: begin without a line number, wrapped to fit inside the window.

![tip47](images/tip47.png)

`j, k, 0, $`: interact with real lines.
`g`: tell vim to act on display lines instead.

# [Tip46](tip46.md) [Tip48](tip48.md)
