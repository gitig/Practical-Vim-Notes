# Tip37: Group Buffers into a Collection with the Argument List  
  
`vim *.txt` then:  
![tip37_1](images/tip37_1.png)  
>the **argument list** represents the list of files that was passed as an argument when we ran the vim command.  
>`[]`: indicate which of the files in the argument list is active.  
  
**Populate the Argument List**  
>When the `:args` is run without arguments, it prints the contents of the argument list.  
  
## :args {arglist}  
>set the contents of the argument list.  
>{arglist} can include filenames, wildcards, or even the output from a shell command.  
  
  
**Specify Files by Name**  
  
![tip37_2](images/tip37_2.png)  
  
**Specify Files by Glob**  
  
## *  
>match zero or more characters, but only in the scope of the specified directory.  
  
## **  
>match zero or more characters, but it can recurse downward into directories below the specified directory.  
  
![tip37_3](images/tip37_3.png)
  
## :args **/*.js **/*.css  
>build an argument list containing all .js and .css files but not other file types.  
  
  
**Specify Files by Backtick Expansion**  
  
![tip37_4](images/tip37_4.png)  
  
# [Tip36](tip36.md) [Tip38](tip38.md)
