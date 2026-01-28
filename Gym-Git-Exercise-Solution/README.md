# Git Exercises
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

