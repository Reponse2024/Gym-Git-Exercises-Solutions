# Git Exercises
## Bundle 1
### Exercise 1

```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ touch Hello.java

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git branch -m master

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (master)                                    
$ git branch -m main

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)                                      
$ git remote add origin https://github.com/Reponse2024/Gym-Exercise-Solutions-Test-Sol.git
git branch -M main
git push -u origin main
error: remote origin already exists.
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 2 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (16/16), 2.20 KiB | 21.00 KiB/s, done.
Total 16 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
   cdff9c6..0011214  main -> main
branch 'main' set up to track 'origin/main'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)                                      
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)                                      
$ git commit -m "Created a Hello file"
[main 8781e64] Created a Hello file
 1 file changed, 2 insertions(+), 1 deletion(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)                                      
$ git push
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (7/7), 585 bytes | 97.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
   0011214..8781e64  main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)                                      
$ git checkout -b dev
Switched to a new branch 'dev'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)                                       
$ git checkout -b test
Switched to a new branch 'test'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (test)                                      
$ git checkout dev
Switched to branch 'dev'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)                                       
$ git branch -d test
Deleted branch test (was 8781e64).

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)                                       
$ 
```
### Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)
$ touch home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)
$ git add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash
Saved working directory and index state WIP on dev: 8781e64 Created a Hello file

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash list
stash@{0}: WIP on dev: 8781e64 Created a Hello file

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ touch about.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git add about.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash
Saved working directory and index state WIP on dev: 8781e64 Created a Hello file

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ touch team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git add team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash
Saved working directory and index state WIP on dev: 8781e64 Created a Hello file

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash list
stash@{0}: WIP on dev: 8781e64 Created a Hello file
stash@{1}: WIP on dev: 8781e64 Created a Hello file
stash@{2}: WIP on dev: 8781e64 Created a Hello file

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../.idea/
        ../manage/

Dropped stash@{1} (3088c691d170033b7b055289b87a5e78f0626c51)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../.idea/
        ../manage/

Dropped stash@{1} (04c0af3c2adf34e768896ca9b12a376c2738e3b9)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git commit -m "Stash popped about and the home pages"
[dev 8798704] Stash popped about and the home pages
 3 files changed, 88 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/about.html
 create mode 100644 Gym-Git-Exercise-Solution/home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ it push --set-upstream origin dev
bash: it: command not found

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../.idea/
        ../manage/

Dropped refs/stash@{0} (5cd7aca364cbca0e3b2e806e81a4ec63c18ad1cf)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git reset --hard
HEAD is now at 8798704 Stash popped about and the home pages

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git commit -m "Reset the changes of stash popping for tea
m.html"
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../.idea/
        ../manage/

nothing added to commit but untracked files present (use "git add" to track)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (dev)               
$ git push --set-upstream origin dev
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.42 KiB | 18.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/dev
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
```

## Bundle 2
### Exercise 1
```bash

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/bundle-2)
$ touch services.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/bundle-2)       
$ git add services.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/bundle-2)       
$ git commit -m "Created and modified a services file"
[ft/bundle-2 1864727] Created and modified a services file
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/services.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/bundle-2)       
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/bundle-2)       
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 631 bytes | 24.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

```

### Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ touch service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git add service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git commit -m "Added Services"
[ft/service-redesign aaf64c0] Added Services
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 616 bytes | 123.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git add service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git commit -m "Modified a file's heading"
[ft/service-redesign 6e32355] Modified a file's heading
 1 file changed, 1 insertion(+), 1 deletion(-)
User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 441 bytes | 63.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
   aaf64c0..6e32355  ft/service-redesign -> ft/service-redesign

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git checkout main
M       Gym-Git-Exercise-Solution/pom.xml
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ touch service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git add services.html
fatal: pathspec 'services.html' did not match any files

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git add service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git commit -m "Added service file in the main branch"
[main f72fc7b] Added service file in the main branch
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git push
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git checkout ft/service-redesign
M       Gym-Git-Exercise-Solution/pom.xml
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git diff main..ft/service-redesign
diff --git a/Gym-Git-Exercise-Solution/service.html b/Gym-Git-Exercise-Solution/service.html
index 35ccd72..778aa81 100644
--- a/Gym-Git-Exercise-Solution/service.html
+++ b/Gym-Git-Exercise-Solution/service.html
@@ -5,9 +5,9 @@
     <meta name="viewport"
           content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
:
diff --git a/Gym-Git-Exercise-Solution/service.html b/Gym-Git-Exercise-Solution/service.html
index 35ccd72..778aa81 100644
--- a/Gym-Git-Exercise-Solution/service.html
+++ b/Gym-Git-Exercise-Solution/service.html
@@ -5,9 +5,9 @@
     <meta name="viewport"
           content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
:
diff --git a/Gym-Git-Exercise-Solution/service.html b/Gym-Git-Exercise-Solution/service.html
index 35ccd72..778aa81 100644
--- a/Gym-Git-Exercise-Solution/service.html
+++ b/Gym-Git-Exercise-Solution/service.html
@@ -5,9 +5,9 @@

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        Gym-Git-Exercise-Solution/service.html
Please commit your changes or stash them before you switch branches.
Aborting

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git pull origin main
fatal: unable to access 'https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git/': Could not resolve host: github.com

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git add .
warning: in the working copy of 'Gym-Git-Exercise-Solution/pom.xml', LF will be replaced by CRLF the next time Git touches it

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git commit -m "Moddified services in service redesign branch"
[ft/service-redesign b23b9d8] Moddified services in service redesign branch
 2 files changed, 2 deletions(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git merge ft/service-redesign
Auto-merging Gym-Git-Exercise-Solution/service.html
CONFLICT (add/add): Merge conflict in Gym-Git-Exercise-Solution/service.html
Automatic merge failed; fix conflicts and then commit the result.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 916 bytes | 61.00 KiB/s, done.
From https://github.com/Reponse2024/Gym-Git-Exercises-Solutions
   8781e64..34f46aa  main       -> origin/main
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...
Vim: Finished.

error: there was a problem with the editor 'vi'
Not committing merge; use 'git commit' to complete the merge.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main|MERGING)
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main|MERGING)
$ git commit -m "Pulled latest changes"
[main 936ca14] Pulled latest changes

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git push
Enumerating objects: 26, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 2 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (16/16), 1.57 KiB | 114.00 KiB/s, done.
Total 16 (delta 8), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (8/8), completed with 3 local objects.
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
   34f46aa..936ca14  main -> main
```
## Bundle 3
### Exercise 1
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)
$ touch team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git add team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git commit -m "Added a team file"
[ft/team-page c72767a] Added a team file
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git push --set-upstream origin ft/team-page
Enumerating objects: 38, done.
Counting objects: 100% (36/36), done.
Delta compression using up to 2 threads
Compressing objects: 100% (29/29), done.
Writing objects: 100% (29/29), 5.64 KiB | 9.00 KiB/s, done.
Total 29 (delta 12), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (12/12), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/ft/team-page
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git checkout main
M       Gym-Git-Exercise-Solution/README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git checkout ft/team-page
M       Gym-Git-Exercise-Solution/README.md
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git log
commit c72767a9e3d1375426e68aea1c53c14168d87d45 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Wed Jan 28 17:52:50 2026 +0200
commit c72767a9e3d1375426e68aea1c53c14168d87d45 (HEAD -> ft
/team-page, origin/ft/team-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Wed Jan 28 17:52:50 2026 +0200

    Added a team file

commit a50b4e7c13270326f894bdc53b396af8e814b744 (origin/main, origin/HEAD, main, ft/contact-page)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/team-page)      
$ git checkout ft/contact-page
M       Gym-Git-Exercise-Solution/README.md
Switched to branch 'ft/contact-page'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git cherry-pick c72767a9e3d1375426e68aea1c53c14168d87d45
[ft/contact-page 3d2343d] Added a team file
 Date: Wed Jan 28 17:52:50 2026 +0200
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ touch contact.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git add contact.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git commit -m "Modified contact page"
[ft/contact-page adee21c] Modified contact page
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/contact.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 2 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 936 bytes | 40.00 KiB/s, done.
Total 8 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/ft/contact-page
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/contact-page)   
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ touch faq.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git add faq.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git commit -m "Modified faq html file"
[ft/faq-page 6e23e68] Modified faq html file
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/faq.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 589 bytes | 84.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git revert c72767a9e3d1375426e68aea1c53c14168d87d45
[ft/faq-page 1d3dd8a] Revert "Added a team file"
 1 file changed, 13 deletions(-)
 delete mode 100644 Gym-Git-Exercise-Solution/team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git commit -m "Reverted team.html"
[ft/faq-page 431f02b] Reverted team.html
 1 file changed, 1 deletion(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)       
$ git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 2 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 736 bytes | 22.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
   6e23e68..431f02b  ft/faq-page -> ft/faq-page
```
### Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        Gym-Git-Exercise-Solution/README.md
Please commit your changes or stash them before you switch branches.
Aborting

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git  add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        Gym-Git-Exercise-Solution/README.md
Please commit your changes or stash them before you switch branches.
Aborting

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git commit -m "Made some changes"
[ft/home-page-redesign 02488af] Made some changes
 2 files changed, 202 insertions(+)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git add service.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git commit -m "Modified serives file"
[main b58a458] Modified serives file
 1 file changed, 2 insertions(+)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git push
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git rebase main
Auto-merging Gym-Git-Exercise-Solution/service.html
CONFLICT (content): Merge conflict in Gym-Git-Exercise-Solution/service.html
error: could not apply 02488af... Made some changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
hint: Disable this message with "git config set advice.mergeConflict false"
Could not apply 02488af... # Made some changes

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase --continue 
Gym-Git-Exercise-Solution/service.html: needs merge
You must edit all merge conflicts and then
mark them as resolved using git add

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase --skip
Successfully rebased and updated refs/heads/ft/home-page-redesign.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ touch home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git  add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git commit -m "ft/created a home page"
[ft/home-page-redesign f0c0e63] ft/created a home page
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 31, done.
Counting objects: 100% (31/31), done.
Delta compression using up to 2 threads
Compressing objects: 100% (27/27), done.
Writing objects: 100% (27/27), 2.87 KiB | 49.00 KiB/s, done.
Total 27 (delta 11), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (11/11), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Reponse2024/Gym-Git-Exercises-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

```
## Bundle 4
### Exercise 1
```bash

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git remote add git-copy https://github.com/Reponse2024/Git-exercise-bundle4-repo.git
error: remote git-copy already exists.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)
$ git remote add git-copyy https://github.com/Reponse2024/Git-exercise-bundle4-repo.git

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ git remote -v
git-copy        https://github.com/Reponse2024/Git-Exercise-Solution-Bundle4-Repo.git (fetch)
git-copy        https://github.com/Reponse2024/Git-Exercise-Solution-Bundle4-Repo.git (push)
git-copyy       https://github.com/Reponse2024/Git-exercise-bundle4-repo.git (fetch)
git-copyy       https://github.com/Reponse2024/Git-exercise-bundle4-repo.git (push)
origin  https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git (fetch)
origin  https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git (push)

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ touch home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ git commit -m "Update the home page content"
[main 5345897] Update the home page content
 1 file changed, 13 insertions(+)
 create mode 100644 Gym-Git-Exercise-Solution/home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ git push origin main
To https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Reponse2024/Gym-Git-Exercises-Solutions.git'                   
hint: Updates were rejected because the remote contains work that you do not                                          
hint: have locally. This is usually caused by another repository pushing to                                           
hint: the same ref. If you want to integrate the remote changes, use                                                  
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.                                            

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$ git push git-copyy main
Enumerating objects: 67, done.
Counting objects: 100% (67/67), done.
Delta compression using up to 2 threads
Compressing objects: 100% (58/58), done.
Writing objects: 100% (67/67), 9.96 KiB | 113.00 KiB/s, done.
Total 67 (delta 21), reused 3 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (21/21), done.
To https://github.com/Reponse2024/Git-exercise-bundle4-repo.git
 * [new branch]      main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (main)              
$
```


