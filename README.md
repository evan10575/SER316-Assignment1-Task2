Number Guessing Game Documentation



Branches at Start of Project



main

* Initial version of number guessing game
* Basic functionality where player guesses a random number between 1-100



dev

* Originates from main
* Adds encouraging message for players after guesses



feature1

* Adds feature that lets players quit by entering a negative number
* Adds play-again loop functionality
* Improves user feedback for guesses



feature2

* Implements a max attempts feature
* Players lose if they run out of guesses



feature3

* Implements a hint system after 3 attempts



hotfix

* Fixed a critical bug for randomInt to properly include max value in range



Task 2 Ending Summary



Differences between merge, squash, rebase, and cherry-pick



Merge

* Best at showing an accurate history, and when the branch is being worked on by multiple members at once
* Allows users to see the specific point when a feature was integrated into the main branch
* May make the history harder to follow as there are lots of merge commits



Rebase

* Creates a cleaner, more linear history by rewriting the commits
* Should never be used when multiple people are working on the same branch



Squash

* Combines multiple commits into one
* Best to use when the commit history is too messy
* Only downside is losing individual details in commit history



Cherry-Pick

* Applies commits to another branch
* Allows user to pick one specific commit and apply it to a branch as opposed to merge/rebase which apply multiple commits at once



Observations in Git History



Feature1 (Merge Strategy) - merged dev into feature1, then merged feature1 into dev. This created a merge commit 66cf59e in the history. It's clearly visible where feature1 branched off and merged back in. Still shows all 4 commits for feature1 in the history.



Feature2 (Rebase Strategy) - rebased feature2's commits onto dev. This created a more linear history with commits 626c8e6 and befa2a0 stacked onto dev. The commit ef689c2 shows that feature2 was merged into dev. The history is slightly cleaner than feature1, but it does not display the branching off point for feature2.



Feature3 (Squash Strategy) - squashed 4 commits into 1 commit e10bde2. Feature3 was then rebased onto dev, this created the cleanest history out of the three feature branches.

