# Git Exercises
## Bundle 2
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
$ git add/rm service.html
git: 'add/rm' is not a git command. See 'git --help'.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase --continue 
Gym-Git-Exercise-Solution/service.html: needs merge
You must edit all merge conflicts and then
mark them as resolved using git add

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rm -fr ".git/rebase-merge
> 
> ^C

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rm -fr ".git/rebase-merge
> ^C

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rm -fr ".git/rebase-merge

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rm -fr .git/rebase-merge
fatal: pathspec '.git/rebase-merge' did not match any files

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase --continue 
Gym-Git-Exercise-Solution/service.html: needs merge
You must edit all merge conflicts and then
mark them as resolved using git add

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign|REBASE 6/6)
$ git rebase --skip
Successfully rebased and updated refs/heads/ft/home-page-redesign.

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ touch home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ git  add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ gir commit -m "ft/created a home page"
bash: gir: command not found

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

User@DESKTOP-PQL5SE4 MINGW64 ~/IdeaProjects/Gym-Git-Exercises-Solutions/Gym-Git-Exercise-Solution (ft/home-page-redesign)
$ 
```
