Stash
============

1.Add stash
--------
*   add change first: `git add change_file"` <br>
*   add stash from staged files: `git stash save "stash message"` <br>

2.List existed stash
--------
*   list stash: `git stash list"` <br>

3.use stash
--------
*   use latest stash: `git stash apply"` <br>
*   use latest stash and delete it: `git stash pop"` <br>
*   use assigned stash: `git stash apply @stash{"stash number"}"` <br>

3.delete stash
--------
*   delete latest stash: `git stash drop"` <br>
*   delete assigned stage stash: `git stash drop @stash{"stash number"}"` <br>
*   delete all stash: `git stash clear"` <br>