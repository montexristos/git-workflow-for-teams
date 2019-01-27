## Cherry-pick

There are cases that we want to merge a single commit back to a branch but avoid merging all other commits included in the branch. 

This can be really useful when we want to merge bug fixes made in the current release of a product/project to a previous version with different codebase. 

In this case if the bugfix branch was created from a working branch that already includes new features, when merged to the old release branch, additional code segments will be merged to.
 
This will result in breaking the old release branch

To avoid this we can use cherry pick. Cherry-pick takes a single commit and tries to merge it to the branch (provided that there are no major changes in affected files). 

Now let’s assume that a commit that fixes a bug in release-2.0/bugfix/bugfix-5 has the sha '43dsn3’. Cherry-pick can be accomplished with the following command:

`git checkout release-1.0/develop`

`git cherry-pick 43dsn3`