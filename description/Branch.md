Branch
============

1.About Branch
--------
Branch is just like a pointer to record the position of node. <br>
`master` is the latest local branch and `origin` is the latest remote branch. <br>
*   HEAD <br>
&ensp; &ensp; &ensp; HEAD is a pointer pointing at the current committed node, and we can check its position by `cat .git/HEAD` <br>
*   Search for branch <br>
&ensp; &ensp; &ensp; list all local branch: `git branch` <br>
&ensp; &ensp; &ensp; list all local and remote branch: `git branch -a` <br>
*   Create a new branch <br>
&ensp; &ensp; &ensp; create new branch at HEAD: `git branch "new_branch_name"` <br>
&ensp; &ensp; &ensp; create new branch at specific position: `git branch "new_branch_name" "hash_or_branch_name"` <br>
*   Delete a branch <br>
&ensp; &ensp; &ensp; delete a merged branch: `git branch -d "branch_name"` <br>
&ensp; &ensp; &ensp; delete a unmerged branch: `git branch -D "branch_name"` <br>
&ensp; &ensp; &ensp; delete a remote branch: `git push origin :"branch_name"` <br>
   

2.Branch Rollback and Switch
--------
`HEAD^^^` and `HEAD~3` mean the position which is three committed nodes away from HEAD.
*   Reset: reset will delete the commits <br>
&ensp; &ensp; &ensp; clean the staged file: `git reset HEAD` <br>
&ensp; &ensp; &ensp; clean the committed file: `git reset HEAD^` <br>
&ensp; &ensp; &ensp; clean the committed file and reset working tree(your file): `git reset HEAD^ --hard` <br>
*   Checkout: checkout just move HEAD to another pointer, but you must create new branch name on original commit otherwise you will not reach the original commit again. <br>
&ensp; &ensp; &ensp; change HEAD to specific committed history: `git checkpoint "hash_or_branch_name"` <br>
&ensp; &ensp; &ensp; create new branch and move HEAD on it: `git checkpoint -b "new_branch_name"` <br>
   

3.Merge
--------
*   Merge <br>
&ensp; &ensp; &ensp; `git checkout master` first and run: `git merge "branch_name"` <br>
*   Conflict <br>
&ensp; &ensp; &ensp; use `git status` find conflict file and modify it, for example: <br>
&ensp; &ensp; &ensp; &ensp; &ensp; &ensp; <<<<<<<HEAD (delete this line) <br>
&ensp; &ensp; &ensp; &ensp; &ensp; &ensp; master branch content (to be modified) <br>
&ensp; &ensp; &ensp; &ensp; &ensp; &ensp; ===================== (delete this line) <br>
&ensp; &ensp; &ensp; &ensp; &ensp; &ensp; other branch content (to be modified) <br>
&ensp; &ensp; &ensp; &ensp; &ensp; &ensp; >>>>>>>new-branch (delete this line) <br>
   
