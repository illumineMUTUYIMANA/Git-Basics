# Git exercise
## bandle 1
### Exercise 1
```bash

User@Illumin▒epc MINGW64 ~ (main)
$ mkdir GitBasics

User@Illumin▒epc MINGW64 ~ (main)
$ cd GitBasics

User@Illumin▒epc MINGW64 ~/GitBasics (main)
$ gitninit
bash: gitninit: command not found

User@Illumin▒epc MINGW64 ~/GitBasics (main)
$ cd ..

User@Illumin▒epc MINGW64 ~ (main)
$ cd gitBasics

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git init
Initialized empty Git repository in C:/Users/User/GitBasics/.git/

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ touch README.md

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ code README.MD

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git branch -m main master

User@Illumin▒epc MINGW64 ~/gitBasics (master)
$ git branch -m master main

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git add .

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git commit -m "initial commit"
[main (root-commit) 86c85ce] initial commit
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git remote add origin https://github.com/illumineMUTUYIMANA/Git-Basics.git

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git branch -m main

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git push -u orgin
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git push -u origin
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 246 bytes | 246.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/illumineMUTUYIMANA/Git-Basics.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git branch div

User@Illumin▒epc MINGW64 ~/gitBasics (main)
$ git checkout div
Switched to branch 'div'

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git branch test

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git branch -d test
Deleted branch test (was 86c85ce).

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git status
On branch div
nothing to commit, working tree clean

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ ls
README.md

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ touch home.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ code home.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash push -m "add a home file"
Saved working directory and index state On div: add a home file

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ touch about.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ code about.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash push -m "add about.html file"
No local changes to save

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git add .

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash push -m "add about.html file"
Saved working directory and index state On div: add about.html file

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ touch team.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ code team.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash push -m "add team.html file"
No local changes to save

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git add .

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash push -m "add team.html file"
Saved working directory and index state On div: add team.html file

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git status
On branch div
nothing to commit, working tree clean

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ ls
README.md

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash list
stash@{0}: On div: add team.html file
stash@{1}: On div: add about.html file
stash@{2}: On div: add a home file

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash pop stash@{1}
On branch div
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (80dfc3c8622c034435d56618dfe286a27a0d64e5)

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git status
On branch div
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash list
stash@{0}: On div: add team.html file
stash@{1}: On div: add a home file

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash pop stash@{1}
On branch div
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{1} (027fdb4b4413e1b614a609a6c0c9ae5b118f3428)

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git add .

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git status
On branch div
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   about.html
        new file:   home.html


User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git commit -m "warking on stash"
[div 896e247] warking on stash
 3 files changed, 123 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git push
fatal: The current branch div has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin div

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git push --set-upstream origin div
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.40 KiB | 1.40 MiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'div' on GitHub by visiting:
remote:      https://github.com/illumineMUTUYIMANA/Git-Basics/pull/new/div
remote:
To https://github.com/illumineMUTUYIMANA/Git-Basics.git
 * [new branch]      div -> div
branch 'div' set up to track 'origin/div'.

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git status
On branch div
Your branch is up to date with 'origin/div'.

nothing to commit, working tree clean

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$  git stash list
stash@{0}: On div: add team.html file

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$  git stash
No local changes to save

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git stash pop stash@{0}
On branch div
Your branch is up to date with 'origin/div'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (4991de5e08444903edd5ed171bf662cf403e5136)

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$  git status
On branch div
Your branch is up to date with 'origin/div'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git reset --hard
HEAD is now at 896e247 warking on stash

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git status
On branch div
Your branch is up to date with 'origin/div'.

nothing to commit, working tree clean ```


## Bundle 2
### Exercise 1

User@Illumin▒epc MINGW64 ~/gitBasics (div)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git status
On branch ft/team-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git add .

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$  git touch service.html
git: 'touch' is not a git command. See 'git --help'.

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ touch service.html

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html


User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ code service.html

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git add --all

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git commit -m "add a new file service.html"
[ft/team-page da154e5] add a new file service.html
 2 files changed, 204 insertions(+), 1 deletion(-)
 create mode 100644 service.html

User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@Illumin▒epc MINGW64 ~/gitBasics (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 2.11 KiB | 2.11 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/illumineMUTUYIMANA/Git-Basics/pull/new/ft/team-page
remote:
To https://github.com/illumineMUTUYIMANA/Git-Basics.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
