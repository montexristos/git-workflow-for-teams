## Hotfix in production

When an issue is identified in Production, and a hotfix is required we create a hotfix branch from master in order to resolve it

`git checkout -b hotfix/hotfix-1 production`

`git push -u origin hotfix/hotfix-1`

When ready we can merge to stage in order to test the fix

`git checkout staging`

`git pull origin staging`

`git checkout hotfix/hotfix-1`

`git rebase -i staging`

`git checkout staging`

`git merge --no-ff hotfix/hotfix-1`

`git push origin staging`

When fix is confirmed we merge the fix to master and all other branches

`git checkout production`

`git merge --no-ff staging`

`git push origin production`

`git checkout develop`

`git merge --no-ff hotfix/hotfix-1`

`git push origin develop`

After the hotfix is merged to all branches, it is safe to delete the hotfix branch

`git branch -d hotfix/hotfix-1`

`git push origin :hotfix/hotfix-1`

We can also tag the hotfix as new release when deployed in production

`git tag v1.0.1`

`git push origin v1.0.1`
