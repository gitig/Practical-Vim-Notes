# Tip63: Interact with the System Clipboard  
Besides Vim's built-in put commands, we can sometimes use the system paste command. However, using this can occasionally produce unexpected results when running Vim inside a terminal. We can avoid these issues by enabling the 'paste' option before using the system paste command.  
  
When we use the system paste command in Insert mode, Vim acts as though each character has been typed by hand. When the 'autoindent' option is enabled, Vim preserves the same level of indentation each time we create a new line. The leading whitespace at the start of each line in the clipboard is added on top of the automatic indent, and the result is that each line wanders further and further to the right.  
  
GVim is able to discern when text is pasted from the clipboard and adjust its behavior accordingly, but when Vim runs inside a terminal this information is not available. The 'paste' option allows us to manually warn Vim that we're about to use the system paste command. When the 'paste' option is enabled, Vim turns off all Insert mode mappings and abbreviations and resets a host of options, including 'autoindent'. That allows us to safely paste from the system clipboard with no surprises.  
  
When we're finished using the system paste command, we should disable the 'paste' option again. That means switching back to Normal mode and then running the Ex command `:set paste!`. Don't you think it would be handly if there were a way of toggling this option without leaving Insert mode?  
  
## :set pastetoggle=&lt;f5&gt;  
>sets up the `<f5>` to toggle the paste option on and off.  
  
**Avoid Toggling 'paste' by Putting from the Plus Register**  
If you're running a version of Vim with system clipboard integration, then you can avoid fiddling with the 'paste' option entirely. The Normal mode `"+p` command pastes the contents of the plus register, which mirrors the system clipboard. This command preserves the indentation of the text in the clipboard so you can expect no surprises, regardless of how the 'paste' and 'autoindent' options are set.  
  
# [Tip62](tip62.md) [Tip64](tip64.md)
