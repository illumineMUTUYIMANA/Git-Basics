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