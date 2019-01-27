## Staging testing cycle is complete

When Staging test process is complete and if any issues are only fixed directly there, then the staging branch should be merged in develop and qa branches. 
Here we can just do a fast forward merge

`git checkout develop`

`git pull origin develop`

`git merge staging`

`git push origin develop`


`git checkout qa`

`git pull origin qa`

`git merge staging`

`git push origin qa`

And when a Production release is scheduled

`git checkout staging`

`git pull origin staging`

`git checkout production`

`git merge staging`

`git push origin production`

We can also tag this release in production if we work with tags

`git tag v1.0`

`git push origin v1.0`
