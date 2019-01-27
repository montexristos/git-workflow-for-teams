## Pull requests

Instead of directly pushing to permanent lived branches, users are encouraged (often forced) to only merge feature or bugfix/hotfix branches using pull requests

The steps to perform a pull request are:

1. Create a separate branch for the feature or fix

2. When ready push the branch to the remote repository

3. Then file a pull request
    * Navigate to Repository’s pull request page and click on pull request
    * Select source and destination branch
    * Add a title and description and submit the pull request
4. Other team members then may review the code, discuss it or make more changes
5. When all work is complete the pull request is merged into the develop or release branch
6. In case the changes cannot be merged automatically (due to conflicts with the master branch) the user needs to rebase the branch to master and push the rebased branch. 
The pull request will be updated with the new version of the branch and there will be no conficts to disallow merging.

The rebase procedure is described [here](rebase.md)