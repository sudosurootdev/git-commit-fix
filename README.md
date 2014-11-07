Git Commit Fix
==============


Have merge conflicts? No problem. Just add fixmerge script into ~/bin directory with executable permissions. Make sure ~/bin is in you PATH as well. When you receive a merge conflict and want to commit ONLY THE NEW PARTS (from cherry-pick, merge, rebase, etc), just type: fixmerge


It will check the merge conflicts, and verify that you want to stage the commit, described below.


If you choose `Y` it will remove everything from the HEAD merge conflict, between `<<<<<<< HEAD` all the way to the `======` seperator, for every file that has a conflict. The second part is left, and the commit message at the bottom of the conflict, after `>>>>>>>` is removed. Then everything is automatically added, commited, and you are sent to commit message.
