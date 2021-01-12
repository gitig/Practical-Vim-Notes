# Tip35: Run Commands in the Shell  
  
**Executing Programs in the Shell**  
  
## :!ls (:!{cmd})  
>call `ls` in the current directory.  
>**This is one-off command**  
  
## :ls  
>call Vim's built-in command, shows the contents of the buffer list.  
  
## % (Command-Line)  
>this `%` symbol is shorthand for the current file name.  
  
## :!ruby %  
>if we're working on a Ruby file, we can execute it by this.  
  
## :shell  
>start an interactive shell session. you can execute several commands.  
  
![tip35_1](images/tip35_1.png)  
      
## &lt;C-z&gt;  
>suspend the process that's running Vim and return control to bash.  
  
##  ($) jobs  
>list the jobs.  
  
##  ($) fg  
>resume a suspended job, bringing it back into the foreground.  
  
**Using the Contents of a Buffer for Standard Input or Output**  
  
## :read !{cmd}  
>put the output from the {cmd} into our current buffer.  
  
## :write !{cmd}  
>use the contents of the buffer as standard input for the specified {cmd}  
  
>`:write !sh`, `:write ! sh`: pass the contents of the buffer as standard input to the sh command.  
>`:write! sh`: write the contents of the buffer to a file called sh.  
  
  
**Filtering the Contents of a Buffer Through an External Command**  
  
## :[range]!{cmd/filter}  
>[range]: The lines specified by [range] are passed as standard input for the {comd}, and then the output from {cmd} overwrites the original contents of [range]. or to put it another way.  
  
![tip35_2](images/tip35_2.png)  
  
## :2,$!sort -t',' -k2  
>`-t','`: tell the sort command that fields are separated with commas.  
>`-k2`: to indicate that the second field is to be used for the sort.  
  
## !{motion}  
>drop us into Command-Line mode and prepopulates the [range] with the liens covered by the specified {motion}.  
  
## !G  (:.,$!)  
>place cursor on line 2 and invoke `!G`, vim opens a prompt with the `:.,$!` range set up for us.  
  
  
![tip35_3](images/tip35_3.png)  
      
# [Tip34](tip34.md) [Tip36](tip36.md)
