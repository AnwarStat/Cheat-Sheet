# Git Cheat Sheet with 40+ commands & concepts
## Anwar Hossain
<blod> Data Scientist | Statistician | Quantitative Researcher | Content Creator</bold><br>

Subscribe my Youtube Channel: http://facebook.com/anwar.datascientist  <br>
Follow me on Facebook: http://facebook.com/anwar.datascientist <br> |
Follow me on Twitter: http://twitter.com/anwar_stat <br>
Follow me on Instragram: http://facebook.com/anwarstatjnu <br> |
Follow me on LinkedIn: http://facebook.com/anwarstat <br> |
Follow me on Github: http://facebook.com/anwarstat<hr>

Tired of memorizing git commands? Here is a cheat sheet with 40+ commands to simplify your life.

## 1. Initialize a local repository
```bash
git init <directory>
```
The <directory> is optional. If you don't specify it, the current directory will be used.
## 2. Clone a remote repository
```bash
git clone <url>
```
## 3. Add a file to the staging area
```bash
git add <file>
```
To add all files in the current directory, use . in place of <file>.
```bash
git add .
```
## 4. Commit changes
```bash
git commit -m "<message>"
```
If you want to add all changes made to tracked files & commit
```bash
git commit -a -m "<message>"
```
### or
```bash
git commit -am "<message>"
```
## 5. Remove a file from the staging area
```bash
git reset <file>
```
## 6. Move or rename a file
```bash
git mv <current path> <new path>
```
## 7. Remove a file from the repository
```bash
git rm <file>
```
You can also remove it from staging area only
```bash
using --cached flag
git rm --cached <file>
```
Basic Git Concepts
Default branch name: main
Default remote name: origin
Current branch reference: HEAD
Parent of HEAD: HEAD^ or HEAD~1
Grandparent of HEAD: HEAD^^ or HEAD~2
## 13. Display branches
```bash
git branch
```
Useful flags:
```bash
-a: Display all branches (local & remote)
-r: Display remote branches
-v: Display branches with last commit
```
## 14. Create a branch
```bash
git branch <branch>
```
You can create a branch and switch to it using the checkout command.
```bash
git checkout -b <branch>
```
## 15. Switch to a branch
```bash
git checkout <branch>
```
##  16. Delete a branch
```bash
git branch -d <branch>
```
You can also force delete a branch using the -D flag.
```bash
git branch -D <branch>
```
## 17. Merge a branch
```bash
git merge <branch to merge into HEAD>
```
Useful flags:
```bash
--no-ff: Create a merge commit even if the merge resolves as a fast-forward
--squash: Squash all commits from the specified branch into a single commit
Fast forward Merge
Fast-forward-merge
Non-Fast forward Merge
No-fast-forward-merge
```
It is suggested to not use the --squash flag as it will squash all commits into a single commit, leading to a messy commit history.
## 18. Rebase a branch
Rebasing is the process of moving or combining a sequence of commits to a new base commit
```bash
git rebase <branch to rebase from>
```
## 19. Checkout a previous commit
```bash
git checkout <commit id>
```
## 20. Revert a commit
```bash
git revert <commit id>
```
## 21. Reset a commit
```bash
git reset <commit id>
```
You can also add the --hard flag to delete all changes, but use it with caution.
```bash
git reset --hard <commit id>
```
## 22. Check out the status of the repository
```bash
git status
```
## 23. Display the commit history
```bash
git log
```
## 24. Display the changes to unstaged files
```bash
git diff
```
You can also use the --staged flag to display the changes to staged files.
```bash
git diff --staged
```
## 25. Display the changes between two commits
```bash
git diff <commit id 01> <commit id 02>
```
## 26. Stash changes
The stash allows you to temporarily store changes without committing them.
```bash
git stash
```
You can also add a message to the stash.
```bash
git stash save "<message>"
```
## 27. List stashes
```bash
git stash list
```
## 28. Apply a stash
Applying the stash will NOT remove it from the stash list.
```bash
git stash apply <stash id>
```
If you do not specify the <stash id>, the latest stash will be applied (Valid for all similar stash commands)
You can also use the format stash@{<index>} to apply a stash (Valid for all similar stash commands)
```bash
git stash apply stash@{0}
```
## 29. Remove a stash
```bash
git stash drop <stash id>
```
## 30. Remove all stashes
```bash
git stash clear
```
## 31. Apply and remove a stash
```bash
git stash pop <stash id>
```
## 32. Display the changes in a stash
```bash
git stash show <stash id>
```
## 33. Add a remote repository
```bash
git remote add <remote name> <url>
```
## 34. Display remote repositories
```bash
git remote
```
Add a -v flag to display the URLs of the remote repositories.
```bash
git remote -v
```
## 35. Remove a remote repository
```bash
git remote remove <remote name>
```
## 36 Rename a remote repository
```bash
git remote rename <old name> <new name>
```
## 37. Fetch changes from a remote repository
```bash
git fetch <remote name>
```
## 38. Fetch changes from a particular branch
```bash
git fetch <remote name> <branch>
```
## 39. Pull changes from a remote repository
```bash
git pull <remote name> <branch>
```
## 40. Push changes to a remote repository
```bash
git push <remote name>
```
## 41. Push changes to a particular branch
```bash
git push <remote name> <branch>
```
