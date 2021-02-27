#Challenge1#

git clone https://github.com/Ritam727/git_hero_2021.git 		//cloned the repo to local computer
git checkout -b challenge1		//created a new branch named challenge1
git add Participants.md 		//added the Participants.md to be tracked in git
git status						//checked whether required files were tracked or not
git commit -m "added required changes"		//commit after making changes
git push origin challenge1			//pushed the changes into the challenge1 branch of my copy of th repo

created pull request with name Solved #1

#Challenge2#

git checkout -b challenge2 		//created a new branch named challenge2
git remote add upstream https://github.com/KamandPrompt/git_hero_2021 			//added upstream
git fetch upstream 				//fetched files from upstream
git merge upstream/version1		//merged the files from upstream/version into challenge2

//rest same as above
----last 3 commits----

commit 1a36fcb8ff499300600c89d56830f81afb07b6df (HEAD -> challenge2)
Merge: ebbfa60 2cff590
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 13:14:09 2021 +0530

    Merge remote-tracking branch 'upstream/version1' into challenge2

commit ebbfa607592fe357736b33b0cf002793dbba3ba5 (origin/challenge1, challenge1)
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 13:08:38 2021 +0530

    added required changes

commit d64aeb6fc5052e4a86ae52e7ac0a3bfca7169556 (origin/main, origin/HEAD, main)
Author: Ritam727 <79043763+Ritam727@users.noreply.github.com>
Date:   Sat Feb 27 13:01:30 2021 +0530

    Name added

----

#Challenge3#

git checkout -b challenge3 		//created new branch challenge3
git rebase -i HEAD~4			//merged the last 4 commits
//rest same as above
----last 3 commits----

commit e987a4b235672b3f090311cd8d5e7ced193d62b1 (HEAD -> challenge3, origin/challenge3)
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 14:09:45 2021 +0530

    added required changes
    
    Added Assets
    
    Added sounds
    
    Added congrats

commit d64aeb6fc5052e4a86ae52e7ac0a3bfca7169556 (origin/main, origin/HEAD, main)
Author: Ritam727 <79043763+Ritam727@users.noreply.github.com>
Date:   Sat Feb 27 13:01:30 2021 +0530

    Name added

commit c939228523637454420689997d4d5367b03cd283 (upstream/main)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:09:47 2021 +0530

    Ready for the Event

----

#Challenge4#

git checkout -b challenge4 		//created new branch challenge4
git reset HEAD~1
git stash
//made required changes
git status 		//to check whether changes made in file have been tracked or not
git add .
git commit -m "added required changes"
git log
git stash pop
//rest same as above
----last 3 commits----
commit de3b8553ecdb374d52d8d13c3d674acd8b16d72d (HEAD -> challenge4)
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 14:24:54 2021 +0530

    added required changes

commit 0396a18b9db0a8bcf340f1d590e79222bab9b493
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:22 2021 +0530

    Added sounds

commit df6aec8f77c4526b2a904a306d548a887c38f575
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:12 2021 +0530

    Added Assets

----
git status
----status----
On branch challenge4
nothing to commit, working tree clean
----

#Challenge5#
git checkout -b challenge5 
git checkout part1 			//switched to part1 branch
git log

----last 3 commits----

commit de3b8553ecdb374d52d8d13c3d674acd8b16d72d
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 14:24:54 2021 +0530

    added required changes

commit 0396a18b9db0a8bcf340f1d590e79222bab9b493
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:22 2021 +0530

    Added sounds

commit df6aec8f77c4526b2a904a306d548a887c38f575
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:12 2021 +0530

    Added Assets
----
//copied the hash of feature1
git switch challenge5
git cherry-pick {hash of feature1}
//did same thing for the rest of the rest of the features and branches as well
//rest same a above

git log

----last 3 commits----
commit 27bb9b292d2f2856ab1f05dacb31b4a9f62e875b (HEAD -> challenge6, origin/challenge5, challenge5)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:19:09 2021 +0530

    feature3

commit e2906faa78f1e99e700bf8b725a4aa456b2d3d51
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:17:54 2021 +0530

    feature2

commit 21ea5401addd01aae44d492ac2ed3052d88369d1
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:22:42 2021 +0530

    feature1
----

#Challenge6#
git checkout -b challenge6
git log

----commits----
commit 27bb9b292d2f2856ab1f05dacb31b4a9f62e875b (HEAD -> challenge6, origin/challenge5, challenge5)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:19:09 2021 +0530

    feature3

commit e2906faa78f1e99e700bf8b725a4aa456b2d3d51
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:17:54 2021 +0530

    feature2

commit 21ea5401addd01aae44d492ac2ed3052d88369d1
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:22:42 2021 +0530

    feature1

commit de3b8553ecdb374d52d8d13c3d674acd8b16d72d
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 14:24:54 2021 +0530

    added required changes

commit 0396a18b9db0a8bcf340f1d590e79222bab9b493
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:22 2021 +0530

    Added sounds

commit df6aec8f77c4526b2a904a306d548a887c38f575
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:12 2021 +0530

    Added Assets

commit ad024b05bfb73087556d85213ff10d01e0f18720 (origin/challenge1, challenge1)
Author: Ritam727 <b20127@students.iitmandi.ac.in>
Date:   Sat Feb 27 14:09:45 2021 +0530

    added required changes

commit d64aeb6fc5052e4a86ae52e7ac0a3bfca7169556 (origin/main, origin/challenge3, origin/HEAD, main)
Author: Ritam727 <79043763+Ritam727@users.noreply.github.com>
Date:   Sat Feb 27 13:01:30 2021 +0530

    Name added

commit c939228523637454420689997d4d5367b03cd283 (upstream/main)
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
----

git rebase -i {commit-hash of bug1}~
//changed the pick to drop
//similarly for bug2
git push origin challenge6
