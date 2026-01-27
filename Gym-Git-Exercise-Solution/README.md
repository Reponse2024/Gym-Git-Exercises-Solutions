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

