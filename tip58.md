#Tip58: Snap Between Files Using Global Marks  
  
**A global mark is a kind of bookmark that allows us to jump between files.**  
  
**after set a mark** we can snap our cursor back to it with the `{letter} command.**  
  
**By default, global marks are persisted between editing sessions**  
  
##m{letter}  
> to set a mark.  
  
**Set a Global Mark Before Going Code Diving**  
##:vimgrep /fooBar/  
>to find all occurrences of a method called fooBar() in our codebase.  
  
By default, :vimgrep jumps directly to the first match that it finds, which could mean switching to another file.  
At this point, we can use the `<C-o>` command to get back to where we were prior to running :vimgrep.  
  
![tip58](images/tip58.png)  
  
Try to get into a habit of setting a global mark before using any commands that :  
>interact with the quickfix list, such as `:grep`, `:vimgrep`, `:make`  
>interact with the buffer and argument lists, such as `:args {arglist}`, `:argdo`  
  
Note: set a blobal mark any time you see something that you might want to snap back to later.  
  
#[Tip57](tip57.md) [Tip59](tip59.md)

