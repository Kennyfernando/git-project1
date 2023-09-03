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

### Git Branching