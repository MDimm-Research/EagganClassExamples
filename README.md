


















README's are not an advantage of submodules
disadvantage... there is not a path to move directory backwords. that would have to be set up. but it could be manages with using the go back one page action in the browser. this issue will not be a problem in local directories only on github.


at present, only three advantages exist


(1) retain ownership and credit to the author whom you used the program from. 

(2) you can star at a more granular level the things you like.

(3) branches allow you to keep up with others contributions to the master but still keep your local branch.




forks need pull requests.
submodules need branch merges.


http://stackoverflow.com/questions/12514197/convert-a-git-folder-to-a-submodule-retrospectively

open issues:
Can I fetch at top level?
or do I have to cd into that specific submodule dir?

then,
git add --all
git commit -m "added subm"
git push -u origin master


all changes can be found by setting the branch to master. So that though problematic is not an incredibly huge issue at moment.

##future deliverables

taking forever to ...
git remote add origin each repository

deliverable 1a 
```for d in ./*/ ; do (cd "$d" && git remote add origin https://github.com/miketestgit01/$d.git); done```
need to solve the above dir issue ... then this portion will become scalable.

deliverable 1b
need to look into the github api for a create repository issue.

deliverable 2


deliverable last.
updating requres a branch merge. or a fetch git add -all and git push -u origin master. 



the below commands work fine.

```
 for d in ./*/ ; do (cd "$d" && git init); done

for d in ./*/ ; do (cd "$d" && git add --all); done


for d in ./*/ ; do (cd "$d" && git commit -m "added new repository"); done



for d in ./*/ ; do (cd "$d" && git push -u origin master); done


```
he does not know it yet, but I want to auto submodule as a gift my buddies whole github repository. Specigfically his repo's Programming Books, Project Euler, and Random Programs. That way people can star the individual programs he has worked on in those genre's instead of starring the overall folder. 
or they could star the individual program and the overall folder!
ArnoldM904
