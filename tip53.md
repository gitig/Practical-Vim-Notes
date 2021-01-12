# Tip53: Mark Your Place and Snap Back to It  
  
**Set the mark**  
## m{a-zA-Z}  
>marks the current cursor location with the designated letter.  
>lowercase marks are local to each individual buffer.  
>uppercase marks are globally accessible.  
  
**Two Normal mode commands**  
## '{mark}  
>moves to the line where a mark was set, positioning the cursor on the first non-whitespace character.  
  
## `{mark}  
>moves the cursor to the exact position where a mark was set, restoring the line and the column at once.  
  
Note: `mm`, ``m`: make a handy pair. They set the mark m and jump to it.  
  
**Vim's Automatic Marks**  
![tip53](images/tip53.png)  
      
# [Tip52](tip52.md) [Tip54](tip54.md)
