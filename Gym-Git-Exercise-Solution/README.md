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



