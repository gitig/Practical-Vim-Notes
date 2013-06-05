#Tip39: Divide Your Workspace into Split Windows  
  
In Vim's terminology, a window is a viewport onto a buffer.  
We can open multiple windows, each containing the same buffer,  
or we can load different buffers into each window.  
  
##&lt;C-w&gt;s  
>divide window horizontally, which create two windows of equal height.  
  
##&lt;C-w&gt;v  
>split window vertically, which produce two windows of equal width.  
  
Note: you can repeat these commands as often as you like, splitting your workspace again and again in a process that resembles cell division.  
  
![tip39_1](images/tip39_1.png)  
      
Note: Each time we use the `<C-w>s` and `<C-w>v` commands, the two resulting split windows will **contain the same buffer** as the original window was divided.  
  
##:edit  
>load another buffer into the active window.  
  
##&lt;C-w&gt;s :edit {filename}  === :split {filename}
>divide our workspace and then open another buffer in one split window while keeping the existing buffer visible in the other split.  
  
![tip39_2](images/tip39_2.png)  
      
**Changing the Focus Between Windows**  
![tip39_3](images/tip39_3.png)  
  
In fact, `<C-w><C-w>` === `<C-w>w`, you can press the `<Ctrl>` key and hold it while typing `ww`(or `wj` or any others from the table) to change the active window. It's easier to do that.  
  
##:close  
>close the active window.  
  
##:only  
>close all windows except the active one.  
  
![tip39_4](images/tip39_4.png)  
      
**Resizing and Rearranging Windows**  
![tip39_5](images/tip39_5.png)  
      
#[Tip38](tip38.md) [Tip40](tip40.md)
