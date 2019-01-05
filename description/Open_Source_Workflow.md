Open Source Workflow
============

1.Workflow
--------
*   fork on github <br>
*   clone fork repository at your github account <br>
&ensp; &ensp; &ensp; `git clone "fork_repo_url"` <br>
*   add remote upstream and origin <br>
&ensp; &ensp; &ensp; `git remote add upstream "upstream_url"` <br>
&ensp; &ensp; &ensp; `git remote add origin "fork_repo_url"` <br>
*   update local repository to latest version <br>
&ensp; &ensp; &ensp; `git pull upstream master` <br>
*   move to `develop branch`, create your own `branch` and start working.  <br>
&ensp; &ensp; &ensp; `git checkout "develop_branch"` + `git checkout -b "my_branch"` <br>
*   commit your work <br>
&ensp; &ensp; &ensp; `git add "file"` + `git commit` <br>
*   push your work to origin <br>
&ensp; &ensp; &ensp; `git push origin "my_branch"` <br>
*   press ***compare & pull request*** at your fork repository and ***create pull request*** <br>
   

2.Workflow Diagram
--------
<img src="https://github.com/danniefairy/Git_note/blob/master/img/workflow.jpg" width = "500"/>
   
