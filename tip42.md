#Tip42: Open a File by Its Filename Using `:find`  
  
##:find  
>open a file by its name without having to provide a fully qualified path.  
  
**Configure the 'path'**  
>'path' option allows us to specify a set of directories inside of which Vim will search when `:find` command is invoked.  
  
##:set path+=app/**  
>`**`: matches all subdirectories beneath the app/ directory.  
  
**Use `:find` to Look up Files by Name**  
  
##:find Main.js&lt;Tab&gt;  
>after first Tab, vim expands the entire path of the first full match.  
>after second Tab, vim expands the next matching full filepath.  
  
#[Tip41](tip41.md) [Tip43](tip43.md)
