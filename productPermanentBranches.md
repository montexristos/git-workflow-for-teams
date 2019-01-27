## Permanent Branches

A similar approach to project based development can be used here. 

The develop branch is again used for development and a different branch is maintained for every available environment (testing, production etc)

A good practice is to keep the product release vesion as a prefix as portrayed in the branch names below

### release-1.0/develop
The release-1.0/develop branch contains the latest version of the specific release and is considered to have the bleeding edge features but also to be unstable

### release-1.0/qa
The release-1.0/qa branch should reflect the code delivered to qa team for testing of features or fixes on previously reported issues

### release-1.0/staging
In the release-1.0/staging branch is merged the code that has passed testing regarding requirements and acceptance criteria. Reflects the code in staging environment where the client performs testing of fixes and added functionality

### release-1.0/production
This branch always contains the code deployed in production and should be deployable at any time. 
