# Introduction

This repository contains a set of documents that describe a workflow that may help medium/large teams to effectively version their code using git

This workflow is based on some commonly used and documented best practices and should be used along with them

All git workflows for teams are based on branches. Usually there is a master branch that always is deployable and develop, feature or bugfix branches where the new feature development or bug fixing code resides

In our workflow we have some branches that are permanent and others that are temporary and should be deleted after being merged

The branch configuration can be different between projects and products to better reflect the versioning requirements of each type of repository

## Git Workflow for project based development

* [Permanent Branches](permanentBranches.md)
* [Short-live branches](shortLiveBranches.md)

## Use cases
* [Work in a feature](feature.md)
* [Fix a bug identified in QA](bug.md)
* [QA testing cycle is complete](qaTest.md)
* [Staging testing cycle is complete](stagingTest.md)
* [Hotfix in production](hotfix.md)

## Git workflow for product based development

* [Permanent Branches](productPermanentBranches.md)

## Other topics

* [Pull Request](pullRequest.md)
* [Updating branch from main branch](rebase.md)
* [Rebase vs Merge](rebaseVsMerge.md)
* [Cherry-pick](cherryPick.md)
* [Squash commits](squash.md)

## Sources:
http://www.cakedc.com/CakeDC_Git_Workflow.pdf

http://williamdurand.fr/2013/11/20/on-creating-pull-requests/

https://ariejan.net/2011/07/05/git-squash-your-latests-commits-into-one/

https://git-scm.com/book/en/v2/Git-Branching-Rebasing

https://www.atlassian.com/git/tutorials/making-a-pull-request

http://learngitbranching.js.org
