# Tip28: Execute a Command on One or More Consecutive Lines

![tip28_1](images/tip28_1.png)
## :print
>echo the specified lines below Vim's command line.

## :digit (:1)
>move cursor to the specified line.

## :$
>move cursor to the end line of the file.

## :3p
>move cursor to line 3 and echo the content of that line.

## :3d  (3G dd)
>jump to line 3 and delete it.


## :2,5p  (:{start},{end})
>print each line from 2 to 5. and cursor would be left positioned on line 5.

## .
>represent current line.

## :%p
>`%`: represent all the lines in the current file.

## :%s/old/new/
>replace the first occurrence of 'old' with 'new' on each line.


## 2G VG
>make a visual selection
>if we press the `:` key, the command-line prompt will be prepopulated with the range `:'<,'>`: stand for the visual selection.
>and if you press `:'<,'>p`: will print the selection!

## '&lt;
>standing for the first line of the visual selection.

## '&gt;
>standing for the last line of the visual selection.


## :/&lt;html&gt;/,/&lt;\/html&gt;/p  (:{start},{end})
>print the tags.

## :/&lt;html&gt;/+1,/&lt;\/html&gt;/-1p  (:{address}+n)
>print the content of the tag except the tag!
>if `n` is omitted, it defaults to 1.

## :2 && :.,.+3p
>equals to `:2,5p`

![tip28_2](images/tip28_2.png)

# [Tip27](tip27.md) [Tip29](tip29.md)
