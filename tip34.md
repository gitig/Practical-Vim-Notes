# Tip34: Recall Commands from History

Vim records the commands that we enter in Command-Line mode and provides two ways of recalling them:
>1. scrolling through past command-lines with the cursor keys.
>2. dialing up the command-line window.

**: switch to Command-Line mode**

## &lt;UP&gt; &lt;DOWN&gt;
>previous and next Ex command
>**can filter the command by pretype: `:co`**

## &lt;C-p&gt; &lt;C-n&gt;
>previous and next Ex comand
>**can not filter the command, just previous and next comand**

Note: By default, Vim records the last twenty commands, you can set by : `set history=200` in vimrc.

**/ switch to search prompt**
>all keys can use like before.


**Meet the Command-Line Window**

Note: Avoid the Cursor Keys When Recalling Commands from History.
you can create the mapping:
>cnoremap &lt;C-p&gt; &lt;Up&gt;
>cnoremap &lt;C-n&gt; &lt;Down&gt;

## q: (Normal mode)
>meet the command-line window.

Note: The Command-Line window is like a regular Vim buffer, where each line contains an item from our history. `h, j, k, l` can use,  when you press the &lt;CR&gt; key, the contents of the current line are executed as an Ex command.

## merge the command
![tip34_1](images/tip34_1.png)

Press &lt;CR&gt; to execute the `:update | !ruby %` command.

![tip34_2](images/tip34_2.png)

# [Tip33](tip33.md) [Tip35](tip35.md)
