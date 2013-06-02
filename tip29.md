#Tip29: Duplicate or Move Lines Using ':t' and ':m' Commands  
  
![tip29_1](images/tip29_1.png)  
  
##:copy :co :t  (:[range]copy{address})  
>duplicate one or more lines from one part of the document to another.  
  
![tip29_2](images/tip29_2.png)  
make a copy of line 6 and put it below the current line.  
  
![tip29_3](images/tip29_3.png)  
  
Note: `:t.`, `yyp`: duplicate the current line. but:  
>`:t.`: does not use register.(Command-Line Mode)  
>`yyp`: use a register.(Normal Mode)  
  
      
##:move :m (:[range]move {address})  
![tip29_4](images/tip29_4.png)  
  
##dGp replace :'&lt;,'&gt;m$  
>`d`: to delete the visual selection.  
>`G`: to jump to the end of the file.  
>`p`: to paste the text that was deleted.  
  
#[Tip28](tip28.md) [Tip30](tip30.md)
