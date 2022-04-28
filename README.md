# :octocat: 💫 Commands :dizzy: :octocat:
Git commands, additional info repo

Everything about git commands. Lessons from [https://www.1234.mn](https://www.1234.mn)

## Command lists :monocle_face: 😃

`git status` **to display files and paths that are different from current head commit**

`git status -s` **to display files in short way**

`git add *` **to prepare the content staged for the next commit**

`git commit` **to create a new commit containing the current contents of the index and the given log message describing the changes**

`git ls-files -s` **to show what is inside staging area**

`git restore [file_name]` **to restore files to working tree from staging area. use asterisc or dot to many files**

`git restore --staged [file_name]` **to restore files to staging area from commited repo in local. use asterisc or dot to many files**

`git clean -fd` **to remove untracked files in working tree**

`git branch [dev]` **to create new branch called dev**

`git checkout [dev]` **to prepare working on branch called dev**

`git switch [dev]` **to prepare working on branch called dev**

`git branch -a` **to all branches**

`git branch -r` **to all only remote branches**

`git branch -d [branch_name]` **to delete branch**

`git branch -D [branch_name]` **to delete branch by force**

`git remote -v` **to be a little more verbose and show remote url after name**

`git remote add [remote_repo_name] [remote_repo_link]` **to add remote repo by name**

`git remote prune [origin]` **to delete stale references associated with <name>**

`git clone [repo_link]` **to clone a repository into a new directory**

`git fetch [origin_name/branch_name]` **to download objects and refs from another repository to .git/ folder. You can specify origin name or specific branch**

`git merge [origin_name/branch_name]` **to join two or more development histories together**

`git cat-files -p [234efi3kw3]` **to show what is inside in that file with hash**

`git show [234efi3kw3]` **to show what is inside in that file with hash**

`git show-ref` **to list refrences local and remote branches with last commit hash**

`git show-ref [branch_name]` **to list refrence local and remote branche with last commit hash**

`git pull` **to fetch from and integrate with another repository or a local branch** **>git fetch  + >git merge branch_name**

`git push [origin] [branch]` **to update remote refs along with associated objects**

`git push --all` **to update remote refs with all associated objects. with connected upstream and tracking branches**

`git push [origin_name] -d [branch_name]` **to delete remote branch_name. local branch_name stay**