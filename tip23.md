#Tip23: Prefer Operators to Visual Commands Where Possible  

note: Visual mode may be more intuitive than Vim's Normal mode of operation, but it has a weakness: it doesn't always play well with the dot command.  
  
![tip23_1](images/tip23_1.png)  
  
##vit  
>select the inner contents of a tag  
>`it` command is a special kind of motion called a text object.  
  
##U  
>converts the selected characters to uppercase  
  
Running `j.`:  
![tip23_1_1](images/tip23_1_1.png)  
  
#Tip:  
>The Visual mode `U` command has a Normal mode equivalent: `gU{motion}`    

#Discussion  
>`vitU` can be considered as two separate commands: `vit` to make a selection and `U` to transform the selection.  
>`gUit` can be considered as a single command comprise of a operator `gU` and a motion `it`.  
  
![tip23_2](images/tip23_2.png)  
##So, we should prefer operator commands over their equivalents when working through a repetitive set of changes.  

#[Tip22](tip22.md) [Tip24](tip24.md)
