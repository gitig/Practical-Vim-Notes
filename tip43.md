#Tip43: Explore the File System with netrw  
  
##Enable netrw plugin  
>set nocompatible  
>filetype plugin on  
  
**Meet netrw ---Vim's Native File Explorer**  
  
##vim directoryname  
>It's a regular Vim buffer, represents the contents of a directory.  
  
if the cursor is positioned on a filename, the file is loaded into a buffer in the current window, replacing the file explorer.  
  
##-  
##.. &lt;CR&gt;  
>goto parent directory.  
  
##:edit {directory path}  
>open the file explorer  
  
##.  
>stands for the current working directory.  
  
![tip43](images/tip43.png)  
  
#[Tip42](tip42.md) [Tip44](tip44.md)
