## Short-live branches

Short live branches are created for a specific task and are deleted after work on this task in concluded and the branch is fully merged.
The most common short-live branches are described below

### Feature branch

Feature branches are created from develop branch for the development of a specific feature. 
If there is a Jira story related with this feature, the branch should take as name the jira item id  followed by a short but explanatory description of the feature (e.g. feature/JIR-12-logging). 
Otherwise a common naming pattern for feature branches is feature/logging.

An example workflow for developing a feature is described [here](feature.md)

### Bugfix branch

Bugfix branches are created from production/master branch (on order to be able to be merge in all branches) and address a specific issue reported during the testing process. 
After completion of the fix they are merged either back to develop branch to be deployed in the next release or directly back in the qa branch and finally back into develop after the fix has been confirmed

An example workflow for fixing a bug is described [here](bug.md)

### Hotfix branch

Hotfix branches are created from production/master branch and address a specific issue reported in production. 
After completion of the fix they are merged in all other branches and finally back into production after the fix has been confirmed to resolve the issue

An example workflow for making a hotfix is described [here](hotfix.md)

### Release Branch

Release branches can be created just before making a new release and most times are used to commit versioning or configuration changes. 
These branches, if they contain no fixes or features, may not be merged back to the master branch. 
