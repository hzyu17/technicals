##[A vim cheat sheet](https://vimsheet.com/)

## copy a whole file / copy content between files:

1.include another file (:r(read)):
```
vim file1
:r file2
```
[other related](https://www.cs.swarthmore.edu/courses/CS21Labs/s17/docs/vimcopypaste.html)

2. tab edit (copy from another file)
```
vim file1           # open one file in vim
:tabe file2         # open second file as a tab (tabe means tab edit)
yy                  # copy a line (or use 5yy to copy 5 lines, etc)
gt                  # switch tabs (gt means go to tab)
p                   # paste the line(s) you copied into this file
```
