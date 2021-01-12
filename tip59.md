# Tip59: Delete, Yank, and Put with Vim's Unnamed Register  
  
Normally when we discuss cut, copy, and paste, we talk about putting text on a clipboard.  
In Vim's terminology, we don't deal with a clipboard but instead with **register**.  
  
**Transposing Characters**  
## x  
>cuts the character under the cursor, placing a copy of it in the **unnamed register**.  
  
## p  
>pastes the contents of the unnamed register **after** the **cursor position**.  
  
## xp  
>Transpose the next two characters.  
  
![tip59_1](images/tip59_1.png)  
  
**Transposing Lines**  
## dd  
>cuts the current line, placing it into the unnamed register.  
  
## p  
>pastes the contents of the unnamed register **after** the **current line**.  
  
## ddp  
>Transpose the order of this line and its successor.  
  
![tip59_2](images/tip59_2.png)  
  
**Duplicating Lines**  
## yyp  
>duplicates current line.  Does a line-wise copy and paste.  
  
![tip59_3](images/tip59_3.png)  
  
**Oops! I Clobbered My Yank**  
## P  
>paste the contents of our unnamed register **in front of** the **cursor**.  
  
## diw  
>in this case, overwrite the contents of the unnamed register.  
  
![tip59_4](images/tip59_4.png)  
  
# [Tip58](tip58.md) [Tip60](tip60.md)
