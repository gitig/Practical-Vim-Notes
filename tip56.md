# Tip56: Traverse the Change List  
  
**Vim records the location of our cursor after each change we make to a document.**  
  
**change list**  
>Vim maintains a list of the modifications we make to each buffer during the course of an editing session.  
  
## :changes  
>shows that Vim records the line and column number for each change.  
>`g;`, `g,`: traverse backward and forward through the change list.  
  
**Marks for the Last Change**  
  
## `.  
>references the position of the last change.  
  
## `^  
>tracks the position of the cursor the last time that Insert mode was stopped.  
  
# [Tip55](tip55.md) [Tip57](tip57.md)
