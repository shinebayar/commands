# :octocat: 💫 Commands :dizzy: :octocat:
Git commands, additional info repo

Everything about git commands. Lessons from [https://www.1234.mn](https://www.1234.mn)

## Command lists :monocle_face: 😃

`git status` **to display files and paths that are different from current head commit**

`git status -s` **to display files in short way**

`git add *` **to prepare the content staged for the next commit**

`git commit` **to create a new commit containing the current contents of the index and the given log message describing the changes**

`git log` **to show commit logs**

`git log --oneline` **to show commit logs by one lines. show short logs**

`git log --oneline --all --graph` **to show all commit logs by one lines and with graph. show short logs**

`git ls-files -s` **to show what is inside staging area**

`git restore [file_name]` **to restore files to working tree from staging area. use asterisc or dot to many files**

`git restore --staged [file_name]` **to restore files to staging area from commited repo in local. use asterisc or dot to many files**

`git show HEAD~2:[file_name]` **to show file content that is saved before 2 commits. HEAD~3 => to show before 3 commit, HEAD => to show before one commit**

`git restore --source HEAD~2 [file_name]` **to restore files to working directory. That is restored from commited files. HEAD~3 => go to before 3 commit, HEAD => go to before one commit** 

`git restore --source HEAD~2 [file_name] --staged` **to restore files to staging area. That is restored from commited files. HEAD~3 => go to before 3 commit, HEAD => go to before one commit** 

`git reflog` **to show reference log files in local repo**

`git reset --hard [commit-hash]` **to go back specific commit OR to reset current HEAD to the specified state. --hard means both index and working tree. You can get commit-hash using that commands: git log --oneline OR git reflog**

`git reset --hard HEAD@{2}` **to reset current head to specified state. You can HEAD@{2} from >git reflog command. --hard points working directory, staging area and local repo. --mixed points staging area and local repo. --soft points to local repo**

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

`git push -u [origin_name] [branch_name]` **to push branch to remote and create upstream branch. If there is no same branch in remote branch. -u ---> creates automatically upstream branch in remote repo**

`git tag -a v0.0.1 [hash] -m "comment-here"` **to create a tag. -a => annotate creater information. You can leave -a**

`git tag` **to show active tags**

`git tag -l [v0*]` **to show and filter all tags that starts with v0**

`git show [tag-name]` **to show more info about tag**

`git checkout [tag-name]` **to switch to tag. to switch to head of tag created**

`git tag -d [tag-name]` **to delete local tag**

`git push orgin [tag-name]` **to push tags to remote repository**

`git push orgin --tags` **to push all tags to remote repository**

`git push --delete origin [tag-name]` **to delete tag in remote repository**

`git merge --squash [branch-name]` **to create condition that produce a single commit of branch_name's all commit. This allows you to create a single commit on top of the current branch whose effect is the same as merging another branch. but do not actually make a commit. You create last single commit by manual**

`git rebase [main-branch]` **to reapply commits on top of another base tip to make linear history. anti polluted history. When occurs conflict -> to solve conflict in vscode or editor -> add edited files in staging area -> >git rebase --continue -> make comment -> to end rebase operation**

`git rebase -i [branch_name]` **Interactive rebasing. Developer chooses every commit how to rebase**

`git cherry-pick [hash]` **to apply the changes introduced by some existing commits**

`git stash push -am "[comment]"` **Use git stash when you want to record the current state of the working directory and the index, but want to go back to a clean working directory. The command saves your local modifications away and reverts the working directory to match the HEAD commit. -m ---> message. -a ---> for newly created files**

`git stash list` **List the stash entries that you currently have**

`git stash pop` **Remove a single stashed state from the stash list and apply it on top of the current working tree state, i.e., do the inverse operation of git stash push**

`git stash apply 2` **Like pop, but do not remove the state from the stash list. Go to second stash savings by pointing index. Can show index from list command**

`git stash drop 2` **Remove a single stash entry from the list of stash entrie by index. In that command index is 2**

`git stash clear` **Remove all the stash entries**

`git revert [hash]` **Given one or more existing commits, revert the changes that the related patches introduce, and record some new commits that record them. This requires your working tree to be clean**

`git revert [hash]...[hash]` **to revert commits from hash to hash. If there is conflict. You can fix the conflict in vscode. then add staging area. then >git revert --continue. It creates new comment**