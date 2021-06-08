# Tip8: Chunk Your Undos

The `u` key triggers the undo command, which reverts the most recent change.
i{insert some text}<Esc> constitutes a change.
From the moment we enter Insert mode until we return to Normal mode, everything we type (or delete) counts as a single change. So we can make the undo command operate on words, sentences, or paragraphs just by moderating our use of the `<Esc>` key.

If I’m in Insert mode with my cursor at the end of a line, the quickest way to open a new line is to press `<CR>`. And yet I sometimes prefer to press `<Esc>o` just because I anticipate that I might want that extra granularity from the undo command.

# Moving Around in Insert Mode Resets the Change

When I said that the undo command would revert all characters entered (or deleted)	during a trip into Insert mode and back, I was glossing over a small detail. If we use the <Up> , <Down> , <Left> , or <Right> cursor keys while in Insert mode, a new undo	chunk is created. It’s just as though we had switched back to Normal mode to move around with the h , j , k , or l commands, except that we don’t have to leave Insert mode. This also has implications on the operation of the dot command.

# [Tip7](tip7.md)  [Tip9](tip9.md)
