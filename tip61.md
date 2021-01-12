# Tip61: Replace a Visual Selection with a Register  
  
![tip61_1](images/tip61_1.png)  
  
When we use the `p` command in Visual mode, Vim **replace the selection** with the contents of the specified register.  
  
![tip61_2](images/tip61_2.png)  
  
**Swap Two Words**  
![tip61_3](images/tip61_3.png)  
>`de` to cut the word "chips", copying it into the unnamed register.  
>Then we visually select the word **fish**, which we want to replace.  
>`p` put the word "chips" into the document, and the word "fish" is copied into the unnamed register.  
>Then we snap back to the gap and paste the word "fish" from the unnamed register back into the document.  
  
Note: `m{char}`command sets a mark, and the `{char} command jumps to the mark.  
  
# [Tip60](tip60.md) [Tip62](tip62.md)
