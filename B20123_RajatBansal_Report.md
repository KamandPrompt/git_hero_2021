git clone https://github.com/LazyXghost/git_hero_2021.git //clone forked repo
git checkout -b challenge1          //create branch challenge1 and move to it
nano Participants.md               //using nano to edit Participants.md
git add Participants.md           //add participants.md in staging area
git commit -m "first commit"       //commited and took snapshot 
git status                         //to check status 
git push origin challenge1         //push to remote repo

//now created pull request Solved#1









git checkout -b challenge2
git remote add upstream https://github.com/KamandPrompt/git_hero_2021
git fetch upstream        //add upstream repo and fetched from it in local repo
git merge upstream/version1          //merged version1 into challenge2
git log -p -3                    //command to view last 3 commits


----last 3 commits-----
commit 304eff5fa49a30f0b8d2148d1d4291ff9f4f9c83 (HEAD -> challenge2)
Merge: 66bc856 2cff590
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:04:32 2021 +0530

    Merge remote-tracking branch 'upstream/version1' into challenge2

commit 66bc856c2c1f294fb0d13fd73a86c844d9ce75ca (origin/challenge1, challenge1)
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:01:38 2021 +0530

    first commit

commit 2cff590643d11184f1043c6a0a6bff16122127a7 (upstream/version1, origin/version1)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:26:59 2021 +0530

    Added congrats

git add .
git commit -m "merged version1 into challenge2"

                             //now pushed in the origin and created pr Solved#2















git checkout -b challenge3
git rebase -i HEAD~2                    //squashed last 3 commits

                           //now pushed into origin and created pr Solved#3

git log -p -3
---last 3 commits-----
commit a68777fd2a6f7b112105dc0f2f59cde307f122d8 (HEAD -> challenge3, origin/challenge3)
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:01:38 2021 +0530

    first commit
    
    Added Assets
    
    Added sounds
    
    Added congrats

commit c939228523637454420689997d4d5367b03cd283 (upstream/main, origin/main, origin/HEAD, main)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:09:47 2021 +0530

    Ready for the Event

commit b29ed6aae3246c1af6386d6c7772cd17cfae8177
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:57:05 2021 +0530
:...skipping...













git branch                       //to check in which branch we are now
git checkout -b challenge4
git reset HEAD~1                     //uncommmit the last commit
git stash                         //save the current changes
git status                         //to check status after stashing
nano spaceShooter.py
git add spaceShooter.py
git commit -m "uncommented line 24 and 25 in spaceShooter.py"


git log
---last 3 commits-----
commit 0ae37ad17c31ddfb248429e59123bc12ed0e4b6e (HEAD -> challenge4)
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:38:14 2021 +0530

    umcommented line 24 and 25 in spaceShoooter.py

commit c939228523637454420689997d4d5367b03cd283 (upstream/main, origin/main, origin/HEAD, main)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:09:47 2021 +0530

    Ready for the Event

commit b29ed6aae3246c1af6386d6c7772cd17cfae8177
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:57:05 2021 +0530

    Bug2


git status
----status----
On branch challenge4
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	assets/
	congrats.txt
	sounds/
nothing added to commit but untracked files present (use "git add" to track)

git stash pop                       //pop the changes which were stashed earlier
git add Participants.md
git commit -m "poped the stash and then committed"
now pushed to origin and created pr Solved#4

        //i asked on whatsapp if we had to add all the files but i added only
        //participants.md so i closed the pr 
git add .
git commit -m "added all the files initialy fewere added"
        //now i again pushed to origin and created the pr Solved#4















git checkout -b challenge5
git log HEAD..upstream/part1                //to directly check log of part1
git cherry-pick 896880c7091d6650a35b90d19c96a83210150932    //cherry-picked the commit
git log HEAD..upstream/part2
git cherry-pick 03c84856df050bda4976a0f3e0a8671636ee4085
git log HEAD..upstream/part3
git cherry-pick 82302d52c87027709a1f1312a11a4f2f9418477f
                           //now i pushed to origin and created pr Solved#5
















git checkout -b challenge6
git log
commit 327bd7e4de98402d28adb29b8736e49df20468a3 (HEAD -> challenge6, origin/challenge5, challenge5)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:19:09 2021 +0530

    feature3

commit f1084701ec374c56725d4534c893f9fcd33cfcb5
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:17:54 2021 +0530

    feature2

commit 61a44e709057bdc1452e1011b11ac5c1a2537afc
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:22:42 2021 +0530

    feature1

commit afa26842883ef195846d01e7461365ae26ad2d84 (origin/challenge4, challenge4)
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:55:40 2021 +0530

    added all the files initialy fewere added

commit 6853158ab44950ec93d03101f7a12d8b78c439f0
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:44:05 2021 +0530

    poped the stash and then committed

commit 0ae37ad17c31ddfb248429e59123bc12ed0e4b6e
Author: LazyXghost <B20123@students.iitmandi.ac.in>
Date:   Sat Feb 27 15:38:14 2021 +0530

    umcommented line 24 and 25 in spaceShoooter.py

commit c939228523637454420689997d4d5367b03cd283 (upstream/main, origin/main, origin/HEAD, main)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:09:47 2021 +0530

    Ready for the Event

commit b29ed6aae3246c1af6386d6c7772cd17cfae8177
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:57:05 2021 +0530

    Bug2

commit d7daaa752baeb4ce2b89105ca5a0da10ef410a58
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:55:35 2021 +0530

    Created Participants.md

commit 87b6e3417a684fe8d3939fd7da5fbaf89c5d762d
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:53:21 2021 +0530

    Bug1

commit 7d18cdc58f7f9c1194faf0b95bf2ae36264310f0
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:52:48 2021 +0530

    Added proper python code

commit 7d50f61aa876373a46a416c532cdd5e60cb3ad41
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:48:19 2021 +0530

    second commit

commit 638a819205d642f8cc35046a8e373afbbb54cbb5
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Fri Feb 26 19:43:35 2021 +0530

    Initial commit

git rebase -i 87b6e3417a684fe8d3939fd7da5fbaf89c5d762d^   //using git rebase
                                 //now removed the bug1 and bug2 lines
                                 //now pushed to origin and created pr Solved#6
