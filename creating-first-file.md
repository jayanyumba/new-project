this is my 3rd attempt to understanding github 
Using Gitbash to write commands for tracking files:
 cd c:users/user/git(to find the location of the file im using )

User@Jay-pc MINGW64 /c/users/user/git (master)
$ git init(to initialize it as a repository)
Reinitialized existing Git repository in C:/Users/User/Git/.git/
$ git status(a common cmd used to show the status of the file im tracking)
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore.txt
        Employee Salaries.txt
        KCC Logo.png
        index.htm
        secret recipe.htm

nothing added to commit but untracked files present (use "git add" to track)
$ git add index.htm(this allows us to track a specific file)

User@Jay-pc MINGW64 /c/users/user/git (master)
$ git status(to see the new status of the files)
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.htm(this file has been tracked)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore.txt
        Employee Salaries.txt
        KCC Logo.png
        secret recipe.htm

User@Jay-pc MINGW64 /c/users/user/git (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .gitignore.txt
        new file:   Employee Salaries.txt
        new file:   KCC Logo.png
        new file:   index.htm
        new file:   secret recipe.htm
**the above new files are staged and now i want to commit them.
**What is commit in GitHub?
**Commit - committing is the process which records changes in the repository. 

User@Jay-pc MINGW64 /c/users/user/git (master)
$ git commit -m "first commit - committing all files"
[master (root-commit) 7a802b2] first commit - committing all files
 5 files changed, 58 insertions(+)
 create mode 100644 .gitignore.txt
 create mode 100644 Employee Salaries.txt
 create mode 100644 KCC Logo.png
 create mode 100644 index.htm
 create mode 100644 secret recipe.htm

$ git log(shows us every commit made)
commit 7a802b28eb387aeec557a9c13407824110a79429 (HEAD -> master)
Author: Jeremy Anyumba <jayanyumba@gmail.com>
Date:   Tue Apr 25 09:24:05 2023 +0300

    first commit - committing all files
$ git log --oneline(shows an abstracted format)
7a802b2 (HEAD -> master) first commit - committing all files

 $ git commit -m "changd first commit to last commit" --amend(to make changes to a commit use --amend)
[master 48eb333] changd first commit to last commit
 Date: Tue Apr 25 09:24:05 2023 +0300
 5 files changed, 58 insertions(+)
 create mode 100644 .gitignore.txt
 create mode 100644 Employee Salaries.txt
 create mode 100644 KCC Logo.png
 create mode 100644 index.htm
 create mode 100644 secret recipe.htm

User@Jay-pc MINGW64 /c/users/user/git (master)
$ git log --oneline
48eb333 (HEAD -> master) changd first commit to last commit

