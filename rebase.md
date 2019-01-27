## Rebasing branch from main branch

While a user works in a feature branch, the main branch may have receive updates that solve issues, or changes functionality related to that feature. 
The feature branch will not receive the update as it is only merged in the main branch.

In this case it is possible to get all latest changes and reapply all new commits on top using the command:

`git pull --rebase origin develop`

In case there are conflicts these should be resolved by the user and conflicted files need to be added before continuing the rebase

`git add {conflictedFile}`

`git rebase --continue`

If the conflicts cannot be resolved the operation can be stopped and reverted with

`git rebase --abort`
