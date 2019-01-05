Branch
============

1.About Branch
--------
*   HEAD <br>
&ensp; &ensp; &ensp; HEAD is a pointer pointing at the current branch, and we can check its position by `cat .git/HEAD` <br>
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
*   Reset: reset will delete the commits <br>
&ensp; &ensp; &ensp; clean the staged file: `git reset HEAD` <br>
&ensp; &ensp; &ensp; clean the committed file: `git reset HEAD^` <br>
&ensp; &ensp; &ensp; clean the committed file and reset working tree(your file): `git reset HEAD^ --hard` <br>
*   Checkout: checkout just move HEAD to another pointer, but you must create new branch name on original commit otherwise you will not reach the original commit again. <br>
&ensp; &ensp; &ensp; clean the staged file: `git reset HEAD` <br>
1
   
