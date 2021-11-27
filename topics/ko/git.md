## Git

[Git에서 커밋 메시지를 작성하는 명령어는 무엇인가요?](#what-is-the-command-to-write-a-commit-message-in-git)

[Git과 SVN의 차이점은 무엇입니까?](#what-is-difference-between-git-vs-svn)

[Git이란?](#what-is-git)

[Git에서 가장 최근 커밋을 취소하는 방법은 무엇입니까?](#how-to-undo-the-most-recent-commits-in-git)

[Git 포크란 무엇입니까? 포크, 분기 및 복제의 차이점은 무엇입니까?](#what-is-git-fork-what-is-difference-between-fork-branch-and-clone)

[What is the difference between "git pull" and "git fetch"?](#what-is-the-difference-between-git-pull-and-git-fetch)

["풀 리퀘스트"와 "브랜치"의 차이점은 무엇입니까?](#whats-the-difference-between-a-pull-request-and-a-branch)

[중앙 집중식 워크플로는 어떻게 작동합니까?](#how-does-the-centralized-workflow-work)

[로컬 저장소를 업데이트해야 합니다. 어떤 git 명령을 사용할 것인가?](#you-need-to-update-your-local-repos-what-git-commands-will-you-use)

[이전 커밋으로 롤백해야 하며 최근 변경 사항은 신경 쓰지 않습니다. 어떤 명령어를 사용해야 할까요?](#you-need-to-rollback-to-a-previous-commit-and-dont-care-about-recent-changes-what-commands-should-you-use)

["git cherry-pick"이란 무엇입니까?](#what-is-git-cherry-pick)

[Git에서 작업 트리와 인덱스인 HEAD의 차이점을 알려주세요.](#tell-me-the-difference-between-head-working-tree-and-index-in-git)

["git stash"는 언제 사용해야 하나요?](#when-should-i-use-git-stash)

[git에서 이전 커밋을 되돌리는 방법은 무엇입니까?](#how-to-revert-previous-commit-in-git)

[Forking Workflow의 장점 설명](#explain-the-advantages-of-forking-workflow)

[Gitflow 워크플로를 설명해 주시겠습니까?](#could-you-explain-the-gitflow-workflow)

["Rebase Workflow"에 대한 일련의 git 명령을 작성하십시오.](#write-down-a-sequence-of-git-commands-for-a-rebase-workflow)

[Git에서 "HEAD"는 무엇입니까?](#what-is-the-head-in-git)

[파일 시스템에서 파일을 제거하지 않고 git에서 파일을 제거하는 방법은 무엇입니까?](#how-to-remove-a-file-from-git-without-removing-it-from-your-file-system)

["gitstash pop"과 "git stash apply"는 "gitstash 팝"의 git 은 영구적인가요?](#what-is-difference-between-git-stash-pop-and-git-stash-apply)

["git reset"이 일반 영어로 무엇을 하는지 설명할 수 있습니까?](#can-you-explain-what-git-reset-does-in-plain-english)

[두 커밋의 차이점을 확인하기 위해 git 명령을 작성하십시오.](#write-down-a-git-command-to-check-difference-between-two-commits)

[이전 Git 커밋을 수정하는 방법은 무엇입니까?](#how-to-amend-older-git-commit)

[특정 파일의 특정 줄을 누가 변경했는지 알기 위해 어떤 git 명령을 사용해야 합니까?](#what-git-command-do-you-need-to-use-to-know-who-changed-certain-lines-in-a-specific-file)

["git merge" 대신 "git rebase"를 언제 사용합니까?](#when-do-you-use-git-rebase-instead-of-git-merge)

[git rebase를 쉽게 취소하는 방법을 알고 있습니까? ](#do-you-know-how-to-easily-undo-a-git-rebase-)



### Git에서 커밋 메시지를 작성하는 명령어는 무엇인가요?

Use:
```sh
git commit -a
```

 -a on the command line instructs git to commit the new content of all tracked files that have been modified. You can use 
```sh
git add <file>
```
or 
```sh
git add -A
```

before git commit -a if new files need to be committed for the first time.


###### Source

* https://www.edureka.co/blog/interview-questions/git-interview-questions/

[[↑] 맨 위로](#Git)
### Git과 SVN의 차이점은 무엇입니까?

The main point in Git vs SVN debate boils down to this: Git is a distributed version control system (DVCS), whereas SVN is a centralized version control system.

###### Source

* https://medium.com/@gauravtaywade/15-interview-questions-about-git-that-every-developer-should-know-bcaf30409647

[[↑] 맨 위로](#Git)
### Git이란?

Git is a Distributed Version Control system (DVCS). It can track changes to a file and allows you to revert back to any particular change.

Its distributed architecture provides many advantages over other Version Control Systems (VCS) like SVN one major advantage is that it does not rely on a central server to store all the versions of a project’s files. 

###### Source

* https://www.edureka.co/blog/interview-questions/git-interview-questions/

[[↑] 맨 위로](#Git)
### Git에서 가장 최근 커밋을 취소하는 방법은 무엇입니까?

```sh
$ git commit -m "Something terribly misguided"      
$ git reset HEAD~                                   # copied the old head to .git/ORIG_HEAD
<< edit files as necessary >>                       
$ git add ...                                       
$ git commit -c ORIG_HEAD                           # will open an editor, which initially contains the log message from the old commit and allows you to edit it
```

###### Source

* https://stackoverflow.com/questions/927358/how-to-undo-the-most-recent-commits-in-git

[[↑] 맨 위로](#Git)
### Git 포크란 무엇입니까? 포크, 분기 및 복제의 차이점은 무엇입니까?

* A **fork** is a remote, server-side copy of a repository, distinct from the original. A fork isn't a Git concept really, it's more a political/social idea. 
* A **clone** is not a fork; a clone is a local copy of some remote repository.  When you clone, you are actually copying the entire source repository, including all the history and branches.
* A **branch** is a mechanism to handle the changes within a single repository in order to eventually merge them with the rest of code. A branch is something that is within a repository. Conceptually, it represents a thread of development.

###### Source

* https://stackoverflow.com/questions/3329943/git-branch-fork-fetch-merge-rebase-and-clone-what-are-the-differences/

[[↑] 맨 위로](#Git)
### "git pull"과 "git fetch"의 차이점은 무엇입니까?

In the simplest terms, `git pull` does a `git fetch` followed by a `git merge`.

* When you use `pull`, Git tries to automatically do your work for you. **It is context sensitive**, so Git will merge any pulled commits into the branch you are currently working in.  `pull` **automatically merges the commits without letting you review them first**. If you don’t closely manage your branches, you may run into frequent conflicts.

* When you `fetch`, Git gathers any commits from the target branch that do not exist in your current branch and **stores them in your local repository**. However, **it does not merge them with your current branch**. This is particularly useful if you need to keep your repository up to date, but are working on something that might break if you update your files. To integrate the commits into your master branch, you use `merge`.

###### Source

* https://stackoverflow.com/questions/292357/what-is-the-difference-between-git-pull-and-git-fetch

[[↑] 맨 위로](#Git)
### "풀 리퀘스트"와 "브랜치"의 차이점은 무엇입니까?

* A **branch** is just a separate version of the code.

* A **pull request** is when someone take the repository, makes their own branch, does some changes, then tries to merge that branch in (put their changes in the other person's code repository).

###### Source

* https://stackoverflow.com/questions/19059838/whats-the-difference-between-a-pull-request-and-a-branch

[[↑] 맨 위로](#Git)
### 중앙 집중식 워크플로는 어떻게 작동합니까?

The **Centralized Workflow** uses a central repository to serve as the single point-of for all changes to the project. The default development branch is called master and all changes are committed into this branch.

Developers start by cloning the central repository. In their own local copies of the project, they edit files and commit changes. These new commits are stored locally.

To publish changes to the official project, developers *push* their local master branch to the central repository. Before the developer can publish their feature, they need to *fetch* the updated central commits and rebase their changes on top of them. 

Compared to other workflows, the Centralized Workflow has no defined pull request or forking patterns. 

###### Source

* https://www.atlassian.com/git/tutorials/comparing-workflows

[[↑] 맨 위로](#Git)
### 로컬 저장소를 업데이트해야 합니다. 어떤 git 명령을 사용할 것인가?

It’s a two steps process. First you fetch the changes from a remote named origin:

```sh
git fetch origin
```
Then you merge a branch master to local:

```sh
git merge origin/master
```
Or simply:

```sh
git pull origin master
```
If origin is a default remote and ‘master’ is default branch, you can drop it eg. `git pull`.

###### Source

* https://samwize.com/2012/10/30/common-git-usage/

[[↑] 맨 위로](#Git)
### 이전 커밋으로 롤백해야 하며 최근 변경 사항은 신경 쓰지 않습니다. 어떤 명령어를 사용해야 할까요?

Let's say you have made mulitple commits, but the last few were bad and you want to rollback to a previous commit:
```sh
git log // lists the commits made in that repository in reverse chronological order
git reset --hard <commit-sha1> // resets the index and working tree
```

###### Source

* https://gist.github.com/chyld/4570933

[[↑] 맨 위로](#Git)
### "git cherry-pick"이란 무엇입니까?

The command git *cherry-pick* is typically used to introduce particular commits from one branch within a repository onto a different branch. A common use is to forward- or back-port commits from a maintenance branch to a development branch.

This is in contrast with other ways such as merge and rebase which normally apply many commits onto another branch.

Consider:
```sh
git cherry-pick <commit-hash>
```

###### Source

* https://stackoverflow.com/questions/9339429/what-does-cherry-picking-a-commit-with-git-mean

[[↑] 맨 위로](#Git)
### Git에서 작업 트리와 인덱스인 HEAD의 차이점을 알려주세요.

* The **working tree/working directory/workspace** is the directory tree of (source) files that you see and edit.
* The **index/staging area** is a single, large, binary file in <baseOfRepo>/.git/index, which lists all files in the current branch, their sha1 checksums, time stamps and the file name - it is not another directory with a copy of files in it.
* **HEAD** is a reference to the last commit in the currently checked-out branch.

###### Source

* https://stackoverflow.com/questions/3689838/whats-the-difference-between-head-working-tree-and-index-in-git

[[↑] 맨 위로](#Git)
### "git stash"는 언제 사용해야 하나요?

The `git stash` command takes your uncommitted changes (both staged and unstaged), saves them away for later use, and then reverts them from your working copy.

Consider:
```sh
$ git status
On branch master
Changes to be committed:
new file: style.css
Changes not staged for commit:
modified: index.html
$ git stash
Saved working directory and index state WIP on master: 5002d47 our new homepage
HEAD is now at 5002d47 our new homepage
$ git status
On branch master
nothing to commit, working tree clean
```
The one place we could use stashing is if we discover we forgot something in our last commit and have already started working on the next one in the same branch:
```sh
# Assume the latest commit was already done
# start working on the next patch, and discovered I was missing something

# stash away the current mess I made
$ git stash save

# some changes in the working dir

# and now add them to the last commit:
$ git add -u
$ git commit --ammend

# back to work!
$ git stash pop
```

###### Source

* https://www.atlassian.com/git/tutorials/saving-changes/git-stash

[[↑] 맨 위로](#Git)
### git에서 이전 커밋을 되돌리는 방법은 무엇입니까?

Say you have this, where C is your HEAD and (F) is the state of your files.
```sh
   (F)
A-B-C
    ↑
  master
```
1. To nuke changes in the commit:
```sh
git reset --hard HEAD~1
```
Now B is the HEAD. Because you used --hard, your files are reset to their state at commit B.
2.  To undo the commit but keep your changes:
```sh
git reset HEAD~1
```
Now we tell Git to move the HEAD pointer back one commit (B) and leave the files as they are and `git status` shows the changes you had checked into C.
3.  To undo your commit but leave your files and your index
```sh
git reset --soft HEAD~1
```
When you do `git status`, you'll see that the same files are in the index as before.

###### Source

* https://stackoverflow.com/questions/927358/how-to-undo-the-most-recent-commits-in-git

[[↑] 맨 위로](#Git)
### Forking Workflow의 장점 설명

The **Forking Workflow** is fundamentally different than other popular Git workflows. Instead of using a single server-side repository to act as the “central” codebase, it gives every developer their own server-side repository. The Forking Workflow is most often seen in public open source projects.

The *main advantage* of the Forking Workflow is that contributions can be integrated without the need for everybody to push to a single central repository that leads to a clean project history. Developers push to their own server-side repositories, and only the project maintainer can push to the official repository.

When developers are ready to publish a local commit, they push the commit to their own public repository—not the official one. Then, they file a pull request with the main repository, which lets the project maintainer know that an update is ready to be integrated.



###### Source

* https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow

[[↑] 맨 위로](#Git)
### Gitflow 워크플로를 설명해 주시겠습니까?

Gitflow workflow employs two parallel *long-running* branches to record the history of the project, `master` and `develop`:
* **Master** -  is always ready to be released on LIVE, with everything fully tested and approved (production-ready).
 * **Hotfix** - Maintenance or “hotfix” branches are used to quickly patch production releases. Hotfix branches are a lot like release branches and feature branches except they're based on `master` instead of `develop`.


* **Develop** - is the branch to which all feature branches are merged and where all tests are performed. Only when everything’s been thoroughly checked and fixed it can be merged to the `master`.
 * **Feature** - Each new feature should reside in its own branch, which can be pushed to the `develop` branch as their parent one.

<div class="text-center">
<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--pLQxGakq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://wac-cdn.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%2520%282%29.svg%3FcdnVersion%3Dji" class="img-fluid" style="max-width: 500px;"/>
</div>


###### Source

* https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

[[↑] 맨 위로](#Git)
### "Rebase Workflow"에 대한 일련의 git 명령을 작성하십시오.

Rebasing replays changes from one line of work onto another in the order they were introduced, whereas merging takes the endpoints and merges them together.

1. Create a feature branch
```sh
$ git checkout -b feature
```
2. Make changes on the feature branch
```sh
$ echo "Bam!" >>foo.md
$ git add foo.md
$ git commit -m 'Added awesome comment'
```
3. Fetch upstream repository
```sh
$ git fetch upstream
```
4. Rebase changes from feature branch onto upstream/master
```sh
$ git rebase upstream/master
```
5.Rebase local master onto feature branch
```sh
$ git checkout master
$ git rebase feature
```
6. Push local master to upstream
```sh
$ git push upstream master
```

Rebasing gives you a clean linear commit history and creates non-obvious benefits to your project if used diligently. Think of it as taking a line of work and pretending it always started at the very latest revision.

###### Source

* http://kensheedlo.com/essays/why-you-should-use-a-rebase-workflow/

[[↑] 맨 위로](#Git)
### Git에서 "HEAD"는 무엇입니까?

`HEAD` is a ref (reference) to the currently checked out commit.

In normal states, it's actually a symbolic ref to the branch you have checked out - if you look at the contents of .git/HEAD you'll see something like "ref: refs/heads/master". The branch itself is a reference to the commit at the tip of the branch. Therefore, in the normal state, HEAD effectively refers to the commit at the tip of the current branch.

It's also possible to have a `detached HEAD`. This happens when you check out something besides a (local) branch, like a remote branch, a specific commit, or a tag. The most common place to see this is during an interactive rebase, when you choose to edit a commit. In detached HEAD state, your HEAD is a direct reference to a commit - the contents of .git/HEAD will be a SHA1 hash.

Generally speaking, HEAD is just a convenient name to mean "what you have checked out" and you don't really have to worry much about it. Just be aware of what you have checked out, and remember that you probably don't want to commit if you're not on a branch (detached HEAD state) unless you know what you're doing (e.g. are in an interactive rebase).

###### Source

* https://stackoverflow.com/questions/2529971/what-is-the-head-in-git

[[↑] 맨 위로](#Git)
### 파일 시스템에서 파일을 제거하지 않고 git에서 파일을 제거하는 방법은 무엇입니까?

If you are not careful during a `git add`, you may end up adding files that you didn’t want to commit. However, `git rm` will remove it from both your staging area (index), as well as your file system (working tree), which may not be what you want.

Instead use `git reset`:
```sh
git reset filename          # or
echo filename >> .gitingore # add it to .gitignore to avoid re-adding it
```

This means that `git reset <paths>` is the opposite of `git add <paths>`.

###### Source

* https://www.codementor.io/citizen428/git-tutorial-10-common-git-problems-and-how-to-fix-them-aajv0katd

[[↑] 맨 위로](#Git)
### "git stash pop"과 "git stash apply"의 차이점은 무엇입니까?

`git stash pop` **throws away** the (topmost, by default) stash after applying it, whereas `git stash apply` **leaves it in the stash list** for possible later reuse (or you can then `git stash drop` it).

This happens unless there are conflicts after `git stash pop` (say your stashed changes conflict with other changes that you’ve made since you first created the stash), in this case, it will not remove the stash, behaving exactly like `git stash apply`.

Another way to look at it: `git stash pop` is `git stash apply && git stash drop`.

###### Source

* https://stackoverflow.com/questions/15286075/difference-between-git-stash-pop-and-git-stash-apply

[[↑] 맨 위로](#Git)
### "git reset"이 일반 영어로 무엇을 하는지 설명할 수 있습니까?

In general, `git reset` function is to take the current branch and reset it to point somewhere else, and possibly bring the index and work tree along.

```sh
- A - B - C (HEAD, master)
# after git reset B (--mixed by default)
- A - B (HEAD, master)      # - C is still here (working tree didn't change state), but there's no branch pointing to it anymore
```

Remeber that in git you have:
* the HEAD pointer, which tells you what commit you're working on
* the working tree, which represents the state of the files on your system
* the staging area (also called the index), which "stages" changes so that they can later be committed together

So consider:
* `git reset --soft` moves HEAD but doesn't touch the staging area or the working tree.
* `git reset --mixed` moves HEAD and updates the staging area, but not the working tree.
* `git reset --merge` moves HEAD, resets the staging area, and tries to move all the changes in your working tree into the new working tree.
* `git reset --hard` moves HEAD and adjusts your staging area and working tree to the new HEAD, throwing away everything.

Use cases:
* Use `--soft` when you want to move to another commit and patch things up without "losing your place". It's pretty rare that you need this.
* Use `--mixed` (which is the default) when you want to see what things look like at another commit, but you don't want to lose any changes you already have.
* Use `--merge` when you want to move to a new spot but incorporate the changes you already have into that the working tree.
* Use `--hard` to wipe everything out and start a fresh slate at the new commit.

###### Source

* https://stackoverflow.com/questions/2530060/can-you-explain-what-git-reset-does-in-plain-english

[[↑] 맨 위로](#Git)
### 두 커밋의 차이점을 확인하기 위해 git 명령을 작성하십시오.

`git diff` allows you to check the differences between the branches or commits. If you type it out automatically, you can checkout the differences between your last commit and the current changes that you have.

```sh
git diff <branch_or_commit_name> <second_branch_or_commit>
```



[[↑] 맨 위로](#Git)
### 이전 Git 커밋을 수정하는 방법은 무엇입니까?

```sh
git rebase -i HEAD^^^
```
Now mark the ones you want to amend with `edit` or `e` (replace `pick`). Now save and exit.

Now make your changes, then:
```sh
git add -A
git commit --amend --no-edit
git rebase --continue
```
If you want to add an extra delete remove the options from the commit command. If you want to adjust the message, omit just the `--no-edit` option.

###### Source

* https://stackoverflow.com/questions/8824971/how-to-amend-older-git-commit/18150592#18150592

[[↑] 맨 위로](#Git)
### 특정 파일의 특정 줄을 누가 변경했는지 알기 위해 어떤 git 명령을 사용해야 합니까?

Use `git blame` - a little feature in git that allows you to see who wrote what in the repository. If you want to know who changed certain lines, you can use the -L flag to figure out who changed those lines. You can use the command: 
```sh
git blame -L <line-number>,<ending-linenumber> <filename>
```

###### Source

* https://github.com/mikeizbicki/ucr-cs100/tree/2015winter/textbook/tools/git/advanced-git

[[↑] 맨 위로](#Git)
### "git merge" 대신 "git rebase"를 언제 사용합니까?

Both of these commands are designed to integrate changes from one branch into another branch - they just do it in very different ways.

Consider before merge/rebase:
```js
A <- B <- C    [master]
^
 \
  D <- E       [branch]
```
after `git merge master`:
```js
A <- B <- C
^         ^
 \         \
  D <- E <- F
```
after `git rebase master`:
```js
A <- B <- C <- D <- E
```

With rebase you say to use another branch as the new base for your work.

**When to use:**
1. If you have any doubt, use merge.
2. The choice for rebase or merge based on what you want your history to look like.

**More factors to consider:**
1. **Is the branch you are getting changes from shared with other developers outside your team (e.g. open source, public)?** If so, don't rebase. Rebase destroys the branch and those developers will have broken/inconsistent repositories unless they use `git pull --rebase`. 
2. **How skilled is your development team?** Rebase is a destructive operation. That means, if you do not apply it correctly, you could lose committed work and/or break the consistency of other developer's repositories.
3. **Does the branch itself represent useful information?** Some teams use the *branch-per-feature* model where each branch represents a feature (or bugfix, or sub-feature, etc.) In this model the branch helps identify sets of related commits. In case of *branch-per-developer* model the branch itself doesn't convey any additional information (the commit already has the author). There would be no harm in rebasing.
4. **Might you want to revert the merge for any reason?** Reverting (as in undoing) a rebase is considerably difficult and/or impossible (if the rebase had conflicts) compared to reverting a merge. If you think there is a chance you will want to revert then use merge.


###### Source

* https://stackoverflow.com/questions/804115/when-do-you-use-git-rebase-instead-of-git-merge

[[↑] 맨 위로](#Git)
### git rebase를 쉽게 취소하는 방법을 알고 있습니까?

The easiest way would be to find the head commit of the branch as it was immediately before the rebase started in the `reflog`

```git
git reflog
```
and to reset the current branch to it (with the usual caveats about being absolutely sure before reseting with the `--hard` option).

Suppose the old commit was `HEAD@{5}` in the ref log:
```git
git reset --hard HEAD@{5}
```

Also rebase saves your starting point to `ORIG_HEAD` so this is usually as simple as:
```git
git reset --hard ORIG_HEAD
```


###### Source

* https://stackoverflow.com/questions/134882/undoing-a-git-rebase

[[↑] 맨 위로](#Git)
