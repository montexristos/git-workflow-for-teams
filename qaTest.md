## QA testing cycle is complete

When QA process is complete then the qa branch should be merged in develop and staging branches.
Here we can just do a fast forward merge

`git checkout develop`

`git pull origin develop`

`git merge qa`

And when a staging release is scheduled

`git checkout qa`

`git pull origin qa`

`git checkout staging`

`git merge qa`

`git push origin staging`
