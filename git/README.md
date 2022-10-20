### Markdown and readme cheatsheet
[CHEATSHEET](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
#### Good habits
When developping on top of an existing package, one can fork this git repo.
#### generate ssh key
[link](https://git-scm.com/book/en/v2/Git-on-the-Server-Generating-Your-SSH-Public-Key)
#### Task lists
Create task list:
```
-[x] task 1
-[] task 2
```
Task lists can also be created in the issue.
#### Mistakenly commit (larger files, forget gitignore, for example)
Best way is to check the commit id by
```
git log
```
and then go back directly to that commit 
```
git reset --hard HEAD~N
```
N is the number of commit you want the HEAD to go back.
