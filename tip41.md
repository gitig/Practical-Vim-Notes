#Tip41: Open a File by Its Filepath Using `:edit`  
  
##:edit  
>open files by an absolute or a relative filepath.  
  
**Open a File Relative to the Current Working Directory**  
  
##:pwd  
>print working directory.  
  
##:edit relative/path/file.ext  
>tab: autocomplete filepath.  
  
**Open a File Relative to the Active File Directory**  
  
##:edit %&lt;Tab&gt;  
>%: shorthand for the filepath of the active buffer.  
>Tab: expand the filepath.  
  
##:edit %:h&lt;Tab&gt;  
>:h : remove the filename while preserving the rest of the path.  
  
Note: a mapping:  
![tip41](images/tip41.png)  
  
#[Tip40](tip40.md) [Tip42](tip42.md)
