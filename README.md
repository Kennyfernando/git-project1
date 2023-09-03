 # Initiializing Git Repository
 franc@Fernandez MINGW64 ~/darey.io
$ mkdir git-project

franc@Fernandez MINGW64 ~/darey.io
$ cd git-project

franc@Fernandez MINGW64 ~/darey.io/git-project
$ git init
Initialized empty Git repository in C:/Users/franc/darey.io/git-project/.git

## Making My First Commit
franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ touch index.txt

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ echo "i am getting to be a devops engr" > index.txt

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ cat index.txt
i am getting to be a devops engr

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git add .
warning: in the working copy of 'index.txt', LF will be replaced by CRLF the
t time Git touches it

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git commit -m "added a new line"
[main (root-commit) cafb75b] added a new line
 1 file changed, 1 insertion(+)
 create mode 100644 index.txt

## Git Branching
### Learning and trying codes on branching in Git
franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git checkout -b project-trial
Switched to a new branch 'project-trial'

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ git branch
  main
* project-trial

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ git switch main
Switched to branch 'main'

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ ls
index.txt

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ cat index.txt
i am getting to be a devops engr

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ vi index.txt

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.txt

no changes added to commit (use "git add" and/or "git commit -a")

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git add .
warning: in the working copy of 'index.txt', LF will be replaced by CRLF the
t

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git commit -m "added a second line"
[main c9d1883] added a second line
 1 file changed, 1 insertion(+)

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git branch
* main
  project-trial

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git checkout project-trial
Switched to branch 'project-trial'

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ ls
index.txt

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ cat index.txt
i am getting to be a devops engr

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ git merge main
Updating cafb75b..c9d1883
Fast-forward
 index.txt | 1 +
 1 file changed, 1 insertion(+)

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ cat index.txt
i am getting to be a devops engr
Am also adding a second line.

franc@Fernandez MINGW64 ~/darey.io/git-project (project-trial)
$ git checkout main
Switched to branch 'main'

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git branch -d project-trial
Deleted branch project-trial (was c9d1883).

# Collaboration And Remote Repositories
1. create a github account
2. create a new repository

### Adding a remote repository to a local repository
copy the link from the github repository
![getting your repo url] (c:\User\franc\Downloads\Screenshot 2023-09-04 002137.jpg)

franc@Fernandez MINGW64 ~/darey.io/git-project (main)
$ git remote add origin https://github.com/Kennyfernando/git-project1.git

