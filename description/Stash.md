Stash
============

1.Add stash
--------
*   add change first: `git add change_file"` <br>
*   add stash from staged files: `git stash save "stash message"` <br>

2.List existed stash
--------
*   list stash: `git stash list"` <br>

3.Use stash
--------
*   use latest stash: `git stash apply"` <br>
*   use latest stash and delete it: `git stash pop"` <br>
*   use assigned stash: `git stash apply @stash{"stash number"}"` <br>

4.Delete stash
--------
*   delete latest stash: `git stash drop"` <br>
*   delete assigned stage stash: `git stash drop @stash{"stash number"}"` <br>
*   delete all stash: `git stash clear"` <br>