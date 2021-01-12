# Tip57: Jump to the Filename Under the Cursor  
  
**Vim treats filenames in our document as a kind of hyperlink. When configured properly, we can use the `gf` command to go to the filename under the cursor.**  
  
## gf  
>go to file  
  
## :set suffixesadd+=.ext  
>`suffixesadd` option allows us to specify one or more file extensions, which Vim will attempt to use when looking up a filename with the `gf` command.  
  
**Specify the Directories to Look Inside**  
We can configure 'path' option to reference a comma-separated list of directories. When we use gf command, Vim checks each of the directories listed in 'path' to see if it contains a filename that matches the text under the cursor.  
  
![tip57_1](images/tip57_1.png)  
  
>`.` stands for the directory of the current file.  
>empty string(delimited by two adjacent commas) stands for the working directory.  
  
# [Tip56](tip56.md) [Tip58](tip58.md)
