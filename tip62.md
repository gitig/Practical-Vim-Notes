#Tip62: Paste from a Register  
##p  
>puts the text from a register **after** the cursor position.  
  
##P  
>puts the text from a register **before** the cursor position.  
  
**Pasting Character-wise Regions**  
Whether we use the `p` or `P` command depends on where the cursor is positioned.  
  
![tip62_1](images/tip62_1.png)  
  
In the first case we would use `p`, whereas in the second case we would use `P`.  
  
##&lt;C-r&gt;{register}  
>paste Character-wise regions of text from Insert mode. The text from the register is always inserted **in front of** the cursor position.  
>`<C-r>"`: insert the contents of the **unnamed register**.  
>`<C-r>0`: insert the contents of the **yank register**.  
  
![tip62_2](images/tip62_2.png)  
  
**Pasting Line-Wise Regions**  
##p P  
>put the text **before** or **after** the current line.  
  
##gp gP  
>put the text **below** or **above** the current line.  
>but they leave the cursor positioned **at the end** of the pasted text instead of at the **beginning**.  
  
![tip62_3](images/tip62_3.png)  
  
`P` would leave our cursor positioned **above** the inserted text.  
`gP` would leave our cursor positioned on the **second duplicate**.  
  
#[Tip61](tip61.md) [Tip63](tip63.md)
