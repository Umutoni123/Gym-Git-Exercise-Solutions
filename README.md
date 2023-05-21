
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

# # Bundle 2
## Exercise 1


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/bundle-2)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/bundle-2)
$ git commit -m "adding the service page and do some changes in It"
[ft/bundle-2 182e943] adding the service page and do some changes in It
 1 file changed, 13 insertions(+)
 create mode 100644 service.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 475 bytes | 237.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/bundle-2
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/bundle-2)
$

## Bundle 2 Exercise 2

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git commit -m "adding the service page and do some changes"
[ft/service-redesign 8cca6ae] adding the service page and do some changes
 1 file changed, 13 insertions(+)
 create mode 100644 service.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 268 bytes | 89.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/service-redesign
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git commit -m "make some changes"
[main 2606c78] make some changes
 1 file changed, 19 insertions(+)
 create mode 100644 service.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 497 bytes | 497.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Umutoni123/bundle-1-exercise-2.git
   b04b81c..2606c78  main -> main

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git diff

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git diff main ft/service-redesign
diff --git a/service.html b/service.html
index 034a007..2085e49 100644
--- a/service.html
+++ b/service.html
@@ -4,16 +4,10 @@
         <title>My web page</title>
     </head>
     <body>
-        <h1>Hello, world! I am making some changes</h1>
-        <h2>Hello, world!</h2>
-        <h3>Hello, world!</h3>
-        <h4>Hello, world!</h4>
-        <h5>Hello, world!</h5>
-        
+        <h1>Hello, world!</h1>
         <p>This is my first web page.</p>
         <p>It contains a
              <strong>main heading</strong> and <em> paragraph </em>.
         </p>
-        
     </body>
 </html>
\ No newline at end of file

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git merge main ft/service-redesign
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign|MERGING)
$ git commit -m "merging and solving the conflicts"
[ft/service-redesign 36975db] merging and solving the conflicts

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 225 bytes | 225.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Umutoni123/bundle-1-exercise-2.git
   8cca6ae..36975db  ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

# Bundle 3 
## Exercise 1


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/team-page)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/team-page)
$ git commit -m "did some changes on team page"
[ft/team-page d8326e1] did some changes on team page
 1 file changed, 13 insertions(+)
 create mode 100644 team.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/team-page)
$ git push -u origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 245 bytes | 81.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/team-page
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.



MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page|REVERTING)
$ git log
commit b04b81cc769fa38404eb73d789a1424adcab4246 (HEAD -> ft/contact-page, main)
Author: noella <noellaumutoni5@gmail.com>
Date:   Mon May 15 11:51:40 2023 +0200

    adding home and about page

commit e76b74ffb4978a2152efb6ac31732a0fb1f384e0
Author: noella <noellaumutoni5@gmail.com>


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page|REVERTING)
$ git cherry-pick  b04b81cc769fa38404eb73d789a1424adcab4246
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit b04b81c.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page|CHERRY-PICKING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page|CHERRY-PICKING)
$ git commit -m "adding a contact page"
[ft/contact-page fd7d788] adding a contact page
 Date: Mon May 15 11:51:40 2023 +0200
 2 files changed, 24 insertions(+)
 create mode 100644 contact.html
 create mode 100644 team.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page|REVERTING)
$ git push -u origin ft/contact-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 547 bytes | 136.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/contact-page
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/contact-page|REVERTING)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git add .


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git commit -m "added faq page"
[ft/faq-page 446aac6] added faq page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git push -u origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 225 bytes | 112.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/faq-page
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git revert b04b81cc769fa38404eb73d789a1424adcab4246
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...
Vim: Finished.
error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git push
Everything up-to-date

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git push -u origin ft/faq-page
Everything up-to-date
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

##  Exercise 2

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/faq-page|REVERTING)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/home-page-redesign|REVERTING)
$ git checkout main
Switched to branch 'main'
D       about.html
D       home.html
Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git commit -m "added a new branch in ft/faq-page branch"
[main 4dfce58] added a new branch in ft/faq-page branch
 2 files changed, 26 deletions(-)
 delete mode 100644 about.html
 delete mode 100644 home.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/home-page-redesign|REVERTING)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/home-page-redesign|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/home-page-redesign|REVERTING)
$ git commit -m "workinf on git rebase and do some changes on home page"
[ft/home-page-redesign 3eca16c] workinf on git rebase and do some changes on home page
 1 file changed, 12 insertions(+)
 create mode 100644 home.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/home-page-redesign|REVERTING)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (10/10), 1.05 KiB | 134.00 KiB/s, done.
Total 10 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/home-page-redesign
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

# Bundle 4
 ## Exercise 1
MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/home-page-redesign|REVERTING)
$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.  
  (use "git pull" to merge the remote branch into yours)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git remote add git-copy  https://github.com/Umutoni123/git-exercises.git


MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git remote
git-copy
origin

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git commit -m "add headers in home page"
[main 43baf4c] add headers in home page
 1 file changed, 16 insertions(+)
 create mode 100644 home.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 766 bytes | 766.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Umutoni123/bundle-1-exercise-2.git
   2606c78..8d16603  main -> main

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git push git-copy main
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (13/13), done.
Writing objects: 100% (16/16), 1.88 KiB | 192.00 KiB/s, done.
Total 16 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/Umutoni123/git-exercises.git
 * [new branch]      main -> main

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git commit -m "add some changes"
[main f8e3e74] add some changes 
 1 file changed, 2 insertions(+)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 340.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Umutoni123/bundle-1-exercise-2.git
   8d16603..f8e3e74  main -> main

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git push git-copy main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 340.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Umutoni123/git-exercises.git
   8d16603..f8e3e74  main -> main
 ## Exercise 2
MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/footer|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/footer|REVERTING)
$ git commit -m "added the ft/footer branch and created the footer page"
[ft/footer 324f59a] added the ft/footer branch and created the footer page
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/footer|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/footer|REVERTING)
$ git commit -m "added some changes on footer page"
[ft/footer e9fa2a6] added some changes on footer page
 1 file changed, 3 insertions(+)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/footer|REVERTING)
$ git push origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 843 bytes | 421.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/footer
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/footer -> ft/footer

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/footer|REVERTING)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/squashing|REVERTING)
$ git merge --squash ft/footer
Updating f8e3e74..e9fa2a6
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 15 +++++++++++++++
 1 file changed, 15 insertions(+)
 create mode 100644 footer.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/squashing|REVERTING)
$ git commit -m "footer changes squashing"
[ft/squashing bef9549] footer changes squashing
 1 file changed, 15 insertions(+)
 create mode 100644 footer.html

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/squashing|REVERTING)
$ git push origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 518 bytes | 518.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Umutoni123/bundle-1-exercise-2/pull/new/ft/squashing
remote:
To https://github.com/Umutoni123/bundle-1-exercise-2.git
 * [new branch]      ft/squashing -> ft/squashing

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/squashing|REVERTING)
$

# Exercise 5
## Exercise 1
MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (ft/squashing|REVERTING)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git add .

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git commit -m "renamed home to index"
[main 02d601e] renamed home to index
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)

MiaBen@Mia MINGW64 /d/bundle1 exercise 2 (main|REVERTING)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 271 bytes | 271.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Umutoni123/bundle-1-exercise-2.git
   f8e3e74..02d601e  main -> main

## Exercise 2


MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git add .

MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git commit -m "added some changes"
[main ecc1930] added some changes
 1 file changed, 1 insertion(+), 1 deletion(-)


MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 313 bytes | 156.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umutoni123/git-cafe-exercise.git
   d1d3f9c..ecc1930  main -> main

# Bundle 6
## Exercise 1

MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git add .

MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git commit -m "added some changes"
[main ecc1930] added some changes
 1 file changed, 1 insertion(+), 1 deletion(-)

MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git push

MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git checkout -b ft/menu
Switched to a new branch 'ft/menu'

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/menu)
$ git add .

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/menu)
$ git commit -m "added menu page"
[ft/menu 7d950a6] added menu page
 1 file changed, 17 insertions(+)
 create mode 100644 menu.html    

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/menu)
$ git push --set-upstream origin ft/menu
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 487 bytes | 243.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote:      https://github.com/Umutoni123/git-cafe-exercise/pull/new/ft/menu
remote:
To https://github.com/Umutoni123/git-cafe-exercise.git
 * [new branch]      ft/menu -> ft/menu
branch 'ft/menu' set up to track 'origin/ft/menu'.

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/menu)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

 ## Exercise 2

MiaBen@Mia MINGW64 /d/git-cafe-exercise (main)
$ git checkout -b ft/bug 
Switched to a new branch 'ft/bug'

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/bug)
$ git add .

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/bug)
$ git commit -m "renamed the index-4 to Contact"
[ft/bug 531c69e] renamed the index-4 to Contact
 1 file changed, 203 insertions(+), 203 deletions(-)
 rename index-4.html => Contact.html (97%)

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/bug)
$ git push origin ft/bug
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.49 KiB | 1.25 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bug' on GitHub by visiting:
remote:      https://github.com/Umutoni123/git-cafe-exercise/pull/new/ft/bug
remote:
To https://github.com/Umutoni123/git-cafe-exercise.git
 * [new branch]      ft/bug -> ft/bug

 ## Exercise 3

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/bug)
$ git add .

MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/bug)
$ git commit -m "changed the phone number"
[ft/bug 9523dfe] changed the phone number
 1 file changed, 1 insertion(+), 1 deletion(-)
 
MiaBen@Mia MINGW64 /d/git-cafe-exercise (ft/bug)
$  git push --set-upstream origin ft/bug
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 297 bytes | 148.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Umutoni123/git-cafe-exercise.git
   531c69e..9523dfe  ft/bug -> ft/bug
branch 'ft/bug' set up to track 'origin/ft/bug'.

