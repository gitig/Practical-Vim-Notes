# Tip20: Grok Visual Mode

**Visual mode**: allows us to select a range of text and then operate upon it.
>Vim has three variants of Visual mode involving working with **characters**, **lines**, **rectangular blocks of text**.

>Many of the commands that you are familiar with from **Normal mode** work just the same in **Visual mode**.like `h`, `j`, `k`, `l`, `f{char}`

## viw
>From Normal mode, we run `viw` to visually select the word.

## c
>`c` command change the selection, deleting the word and dropping us into Insert mode.

**Select mode**: if we type any printable character in Select mode, it will replace the selection and switch to Insert mode. But **Visual mode** doesn't follow this convention! You should run `c` to delete the selection.

# [Tip19](tip19.md) [Tip21](tip21.md)
