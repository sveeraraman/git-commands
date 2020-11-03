Quick Reference Guide for Git commands
----------------------------------

Setup Config properties
----------------------------------

git config --global core.editor "notepad++ -multiInst -nosession"

git config --global -e

git config --global difftool.p4merge.path "C:\Program Files\Perforce\p4merge.exe"

git config --global difftool.p4merge.path "C:/Program Files/Perforce/p4merge.exe"

git config --global merge.tool p4merge

git config --global mergetool.p4merge.path "C:/Program Files/Perforce/p4merge.exe"

git config --global mergetool.prompt false

git config --global difftool.prompt false


Git commands
----------------------------------

git init demo

git status

git add hello.txt (moving to staging area)

git add . (all files)

git init . (to add an existing folder to git)

git log

git show

git ls-files (to get files being tracked)

git commit -a (added files to staging)

git commit -am "updating hello file" (commit added file with inline comment)

git commit -m "init"

git restore --staged Hello.txt (remove from staging)

git checkout -- Hello.txt (revert all changes)

git log --oneline (short logs)

git log --oneline --graph --decorate --all

git config --global alias.hist "log --oneline --graph --decorate --all" (creating git alias command. Here creating a hist command to show log in oneline format)

git config --global --list (to view global configs)

git mv example.txt demo.txt (to rename a file)

git commit -m "renaming example" (commit comment)

git rm demo.txt (removing a file)

git add -u (staging deletes to git)

git add -A (include both addition and deletions)

git difftool HEAD (last commit location. you can also manually move head section)

git difftool

git branch (list current branches)

git checkout -b updates (create and checkout to that branch)

git diff updates master (diff between branches)

git checkout master (switching to master branch)

git merge updates (merge to current branch from updates branch)

git branch -d updates (delete a branch)

git mergetool (run mergetool for conflicts)

git tag mytag (create a tag)

git tag --list (list all tags)

git tag -d mytag (delete a tag)

git tag -a v1.0 -m "Release 1.0" (create annotated tag)

git show v1.0 (show a tagged version)

git stash (saving working directory for stashing)

git stash list (get list of stashes)

git stash pop (applying and dropping a last stash)

git reset ce2c810 --soft (resetting to a previous version --hard all pending changes wiped out/ --soft / --mixed)

git reflog (showses all actions taken on this repo)

git reset --hard (undo all changes)

git statch (discard all local changes but save them for later)

git reset (unstage everything)

-----------------GITHUB-------------------

git remote add origin <git url>

git push -u origin master --tags (push our changes)

git clone ssh url <local folder name>

Create SSH Key
----------------------------------

ssh-keygen -t rsa -C "<youremail>" - Give folder path to store the keys

ssh -T git@github.com
