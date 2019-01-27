## Permanent Branches

A standard approach on branching is to have a develop branch for development and a different branch for every available environment (testing, production etc)

### develop
The develop branch contains the latest version of the code and is considered to have the bleeding edge features but also to be unstable

### qa
The qa branch should reflect the code delivered to qa team for testing of features or fixes on previously reported issues

### staging
In the staging branch is merged the code that has passed testing regarding requirements and acceptance criteria. Reflects the code in staging environment where the client performs testing of fixes and added functionality

### master / production
This branch always contains the code deployed in production and should be deployable at any time. 
