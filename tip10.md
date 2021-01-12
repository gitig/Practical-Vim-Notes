# Tip10: Use Counts to Do Simple Arithmetic  
  
  
`<C-a>`  
>perform addition on numbers.  
  
`<C-x>`  
>perform subtraction on numbers.  
   
   
**comment**: When run without a count they increment by one, but if we prefix a number, we can change by that number. For example, if we positioned our cursor on a `5` character, running `10<C-a>` would modify it to read `15`.  
  

But what happens if the cursor is not positioned on a numeric digit? The documentation says that the `<C-a>` command will **“add [count] to the number at or after the cursor”** (see :h ctrl-a ). So if the cursor is not already positioned on a number, then the `<C-a>` command will look ahead for a digit on the current line. If it finds one, it jumps straight to it. We can use this to our advantage. 
  
## yyp  
>duplicate current line once  
  
## cw  
>delete character under the cursor and change to Insert mode.  
  
## cW  
>delete to the end of the word under the cursor and change to Insert mode.  
  
# Example:  
![tip10](images/tip10.png)  
# Take care:  
>If you answered 008, then you might be in for a surprise when you try using Vim’s `<C-a>` command on any number with a ****leading zero****. As is the convention in some programming languages, Vim interprets numerals with a leading zero to be in octal notation rather than in decimal. In the octal numeric system, `007` + `001` = `010`, which looks like the decimal ten but is actually an octal eight. Confused? If you work with octal numbers frequently, Vim’s default behavior might suit you. If you don’t, you probably want to add the following line to your **vimrc**:  
`set nrformats=`  
This will cause Vim to treat all numerals as decimal, regardless of whether they are padded with zeros.  
  
# [Tip9](tip9.md) [Tip11](tip11.md)
