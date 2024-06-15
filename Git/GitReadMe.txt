Why?
-I intend to improve Linux CLI foundations, and git is an important way of documenting in a workspace before pushing it through to Github.

Starting documentation a bit late into the course.
Better late than never.

Learning importance or *git reset*
!! Helps with a do-over !!



$ git log 
commit 1f4b2b494e95441fa15cd8d8238ffb87df3b3ff7
Author: codecademy <ccuser@codecademy.com>
Date:   Sun Jun 9 15:57:21 2024 +0000

    Mod Scene2

commit 58a40fb72b6a561b9f4849f894edabbdff6ee14c
Author: codecademy <ccuser@codecademy.com>
Date:   Sun Jun 9 00:04:39 2024 +0000

    Add scene 5

commit 7be7ec672af73cf31ef72c92e3374fd4e29c675a
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:15:05 2015 -0500

    Add first page of scene-7.txt

commit 83f7b3591f4ab7aedb3160388b59e65ee1cd94a2
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:14:48 2015 -0500

    Add first page to scene-5.txt

commit 5d692065cf51a2f50ea8e7b19b5a7ae512f633ba
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:14:30 2015 -0500

    Add first page to scene-3.txt

commit 27a3bfe282808aefe69d04f4d111e7a6a0c652dd
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:14:08 2015 -0500

    Add first page to scene-2.txt

commit 96f1625d347d599e6f0f13f23022b3f852d5b116
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:13:38 2015 -0500

*Using first 7 characters of SHA from previous commit, I'm able, so to speak, jump back in time to that commit"


$ git reset 83f7b35
Unstaged changes after reset:
M       scene-2.txt
M       scene-3.txt
M       scene-5.txt


$ git log 
commit 83f7b3591f4ab7aedb3160388b59e65ee1cd94a2
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:14:48 2015 -0500

    Add first page to scene-5.txt

commit 5d692065cf51a2f50ea8e7b19b5a7ae512f633ba
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:14:30 2015 -0500

    Add first page to scene-3.txt

commit 27a3bfe282808aefe69d04f4d111e7a6a0c652dd
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:14:08 2015 -0500

    Add first page to scene-2.txt

commit 96f1625d347d599e6f0f13f23022b3f852d5b116
Author: danasselin <johndoe@example.com>
Date:   Tue Nov 3 17:13:38 2015 -0500

    Add .gitignore



!!HEAD is the most recent commit!!


Thoughts?
-Loving the way I can backtrack using previous commits. Git is dope! I'm glad I'm taking this fundamental course. I feel it already will change the way I document my projects moving forward

COMMANDS USED IN THIS LESSON:
git checkout HEAD filename: Discards changes in the working directory.
git reset HEAD filename: Unstages file changes in the staging area.
git reset commit_SHA: Resets to a previous commit in your commit history.


NOTE: Just because you reset a commit to a previous one, doesn't mean it changed the working directory. That's why git checkout HEAD is a useful command to get you back to your working directory.




*GIT STASH*