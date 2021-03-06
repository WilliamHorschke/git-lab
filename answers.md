Answer 1: git version 2.30.0.windows.2

Answer 2 (git config --list):
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
core.editor="C:\Users\falco\AppData\Local\Programs\Microsoft VS Code\Code.exe" --wait
user.name=William Horschke
user.email=wh477117@ohio.edu

Answer 3: Typing git <command> --help opens up a help page in my browser specifically about the command I entered. Typing git --help (without a command) outputs some help text in the terminal including a list of commands and brief descriptions of what they do. 

Answer 4 (git status before adding):
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        answers.md

nothing added to commit but untracked files present (use "git add" to track)


Answer 5 (git status after adding README.md):
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        answers.md


Answer 6 (git status after adding both files):
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   answers.md


Answer 7 (git status after initial commit, Note that answers.md is modified because I had already began typing this answer):
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")


Answer 8 (git log):
commit 99d14f162bed47f4a517df798324b4a2e8e8ee66 (HEAD -> master)
Author: William Horschke <wh477117@ohio.edu>
Date:   Wed Jan 27 18:42:17 2021 -0500

    Initial commit


Answer 9 (git status after pushing repository to GitHub):
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")


Answer 10: Online changes to README.md are not reflected in the local copy of README.md.

Answer 11: git push gave the following error:
To https://github.com/WilliamHorschke/git-lab.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/WilliamHorschke/git-lab.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.


Answer 12: After using git pull, README.md was updated to match the changes made online.

Answer 13 (directory of git-lab-2 repository output):
Directory of C:\Users\falco\Documents\cs2400\git-lab-2

01/27/2021  07:05 PM    <DIR>          .
01/27/2021  07:05 PM    <DIR>          ..
01/27/2021  07:05 PM               302 .gitignore
01/27/2021  07:05 PM                11 README.md
               2 File(s)            313 bytes
               2 Dir(s)  12,277,780,480 bytes free