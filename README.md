
# Bundle  1
## exercise 1

MiaBen@Mia MINGW64 ~
$ git config --global user.name "noella"

MiaBen@Mia MINGW64 ~
$ git config --global user.email "noellaumutoni5@gmail.com"

MiaBen@Mia MINGW64 ~
$ git config --global init.default branch master

MiaBen@Mia MINGW64 ~
$ cd D:/bundle1

MiaBen@Mia MINGW64 /d/bundle1
$ git init
Initialized empty Git repository in D:/bundle1/.git/

MiaBen@Mia MINGW64 /d/bundle1 (master)
$  git branch -m master main

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        style.css

nothing added to commit but untracked files present (use "git add" to track)

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
        new file:   style.css


MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git commit -m "adding the new files"
[main (root-commit) bf87367] adding the new files
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
 create mode 100644 style.css

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git commit -m "add the content inside the files"
[main b45df14] add the content inside the files
 2 files changed, 20 insertions(+)
 create mode 100644 about.html

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git commit -m "editing the paragragh in about page"
[main 89c47fd] editing the paragragh in about page
 1 file changed, 2 insertions(+), 1 deletion(-)

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git mv about.html service.html

MiaBen@Mia MINGW64 /d/bundle1 (main)


MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git commit -m "renamed the about page to service"
[main bc24106] renamed the about page to service
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename about.html => service.html (100%)

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git remote add origin https://github.com/Umutoni123/bundle1.git

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git push -u origin main
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (11/11), 1.15 KiB | 196.00 KiB/s, done.
Total 11 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Umutoni123/bundle1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

MiaBen@Mia MINGW64 /d/bundle1 (main)
$  git branch dev

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

MiaBen@Mia MINGW64 /d/bundle1 (main)
$  git branch dev main
fatal: a branch named 'dev' already exists

MiaBen@Mia MINGW64 /d/bundle1 (main)
$  git branch test dev

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git branch
  dev
* main
  test

MiaBen@Mia MINGW64 /d/bundle1 (main)
$ git branch -d test
Deleted branch test (was bc24106).

## Exercise 2

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash
Saved working directory and index state WIP on main: e76b74f removed homepage to restart


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash
Saved working directory and index state WIP on main: e76b74f removed homepage to restart

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash
Saved working directory and index state WIP on main: e76b74f removed homepage to restart

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash list
stash@{0}: WIP on main: e76b74f removed homepage to restart
stash@{1}: WIP on main: e76b74f removed homepage to restart
stash@{2}: WIP on main: e76b74f removed homepage to restart



MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (bc89815277ca61265375d2ce4776c62aa64ceb92)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash list
stash@{0}: WIP on main: e76b74f removed homepage to restart
stash@{1}: WIP on main: e76b74f removed homepage to restart

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash pop^C

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (8fb07f4da3e74722c9a602c685ef5a4bb86d9d03)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git commit -m "adding home and about page"
[main b04b81c] adding home and about page
 2 files changed, 26 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 429 bytes | 214.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Umutoni123/bundle-1-exercise-2.git
   e76b74f..b04b81c  main -> main

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash list
stash@{0}: WIP on main: e76b74f removed homepage to restart

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (845a2328c44f10b0c24a2369a401baee108fae12)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git reset --hard
HEAD is now at b04b81c adding home and about page

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$
