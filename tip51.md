# Tip51: Trace Your Selection with Precision Text Objects  
  
## Text Objects  
>define regions of text by structure. It allow us to operate on the regions of text that they delimit.  
  
![tip51_1](images/tip51_1.png)  
  
## vi}  
>Vim initiates Visual mode and then selects all of the characters contained by the {} braces.  
>Where the cursor is positioned to begin with doesn't matter so long as it's located somewhere inside a block of curly braces when the `i}` text object is invoked.  
  
## a"  
>selects a range of characters delimited by double quotes.  
  
>`i`: select **inside** the delimiters.(inside)  
>`a`: select **everything** including the delimiters.(around/all)  
  
![tip51_2](images/tip51_2.png)  
  
Note:  
>Text objects are not motions themselves:  
>we can not use them to navigate around the document.  
>we can use them in Visual mode and in Operator-Pending mode.  
  
**Remember this: whenever you see {motion} as part of the syntax for a command, you can also use a text object.** Common examples include `d{motion}`, `c{motion}`, `y{motion}`.  
  
![tip51_3](images/tip51_3.png)  
>`ci"`: change inside the double quotes.  
>`cit`: change inside the tag.  
>`yit`: yank the text from inside the tag.  
>`dit`: delete the text from inside the tag.  
  
# [Tip50](tip50.md) [Tip52](tip52.md)
