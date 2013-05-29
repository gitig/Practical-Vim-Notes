#Tip24: Edit Tabular Data with Visual-Block Mode  
  
##<C-v>3j  
>`<C-v>`: to engage Visual-Block mode; then we define the column selection by moving our cursor down several lines  

##x...  
>`x` key deletes that column, `.` repeats the deletion for the same range of text.  
  
##gv  
> RESELECT our last visual selection  
  
##r|  
> replace each character in the selection with a pipe character.  
  
##yyp  
> we do a quick line-wise yank-and-put to duplicate the top line.  
  
##Vr-  
> replace every character in that line with a dash character.  
  
![tip24](images/tip24.png)  
  
#[<<Tip23](tip23.md) [Tip25>>](tip25.md)


