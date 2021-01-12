# Tip40: Organize Your Window Layouts with Tab Pages  
  
![tip40_1](images/tip40_1.png)  
  
In Vim, a **tab page** is a container that can hold a collection of windows.  
  
`:edit`: vim doesn't automatically create a new tab.  
Instead, it creates a new **buffer** and loads it into the current window.  
  
## :lcd {path}  
>set the working directory locally for the **current window**, not to the current tab page.  
>a tab page can contains one or more windows.  
  
**Opening and Closing Tabs**  
![tip40_2](images/tip40_2.png)  
      
**Switching Between Tabs**  
Tabs are numbered starting from 1. We can **goto tab{N}**.  
![tip40_3](images/tip40_3.png)  
  
**Rearranging Tabs**  
## :tabmove [N]  
>rearranging tab pages.  
> [N] is 0, the current tab page is moved to the beginning.  
> omit [N], the current tab page is moved to the end.  
  
# [Tip39](tip39.md) [Tip41](tip41.md)
