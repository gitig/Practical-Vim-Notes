# Tip44: Save Files to Nonexistent Directories  
  
## &lt;C-g&gt;  
>echo the name and status of the current file.  
  
When we run the :write command, Vim will attempt to write the contents of that buffer to a new file using the filepath that was specified when the buffer was created.  
  
## :!mkdir -p %:h  
>-p: tell `mkdir` to create intermediate directories.  
  
## :write  
  
# [Tip43](tip43.md) [Tip45](tip45.md)
