#Tip45: Save a File as the Super User  
  
`vim /etc/hosts`: open the hosts file.  
`<C-g>`: echo the status of the file, in this case : [RO]  
`Go`: add a blank line at the end of the file. Vim echoes a message that reads 'W10: Warning: Changing a readonly file.', after showing that message, Vim proceeds by making the change anyway.  
Note: Vim won't prevent us from making changes to a readonly buffer, but it will prevent us from saving the changes to disk.  
  
##:w !sudo tee % &gt; /dev/null  
>`%`: expands to represent the path of the current buffer, in this case: /etc/hosts  
>`tee /etc/hosts > /dev/null`: receives the contents of the buffer as standard input, using it to overwrite the contents of the /etc/hosts file.  
  
#[Tip44](tip44.md) [Tip46](tip46.md)
