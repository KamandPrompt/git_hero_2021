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
git rebase -i HEAD~2			//merged the last 4 commits

----last 3 commits----

commit dace52eb761625c248a10a3529917807c3309882 (HEAD -> challenge3)
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:26:59 2021 +0530

    Added congrats

commit e05bd11cb0b8da5969148728c0fa14423f9f9d95
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:22 2021 +0530

    Added sounds

commit 7070a0599d9f273c8d8547de999b97b29f07b601
Author: Signior-X <b19188@students.iitmandi.ac.in>
Date:   Sat Feb 27 02:25:12 2021 +0530

    Added Assets

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

