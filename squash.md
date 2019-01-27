## Squash commits

It is possible to squash several commits into one if you want to cleanup history in a branch, or if you want all changes in a feature or bugfix branch to be included in a single commit

For example if a user wants to squash the last 2 commits

`git rebase -i HEAD~2`

In the editor he needs to select the commits that he want to squash.

It is also possible to change the commit message of the squashed commit to something that includes all changes.

After all required edits are selected the operation is finalized by hitting save.

**Note:** It is not wise to squash commits that are already pushed to remote.
The branch history will change and this may cause trouble to others working on the same branch.