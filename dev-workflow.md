# Workflow  
  
## Issues
*section needs to be added*

## Git
  
### Branches Overview
-  There are two primary branches shared by the team, `develop` and `master`
-  Development happens on temporary `feature`, `bugfix` and `hotfix` branches
- The `feature`, `bugfix` and `hotfix` are merged into `develop` and `master` when they are ready to deploy

### Commit messages 
- Commit messages should include the issue number, this enables the commit to be tracked to the issue it is coming to resolve
- Commit message should include a brief description of what the commit is accomplishing, feature of fix
   
### Feature 
- When working on a feature, create a branch off of `develop` branch with the feature/ prefix, like so: `feature/<issue-number><feature name>`  
- Once the feature is ready for test merge into `develop` branch  
- Commits to `develop` will deploy to staging server via ci pipeline for client review and testing  
  - Before pushing commits, ensure the code meets standards by running `npm run eslint` and `npm run phpcs`  
  - It is recommended that you setup the `pre-commit` hook to run the above on commit  
  - If code does not meet standards, the deployment will fail  
- Once approved merge feature branch to `master` which deploys to production via ci pipeline  
- Clean up feature branches as they become unneeded  
  
### Bug fix  
- When working on a bug, create a branch off of `develop` branch with the bugfix/ prefix, like so: `bugfix/<issue-number><bug name>`  
- Next steps are similar workflow for feature branch above  
  
### Hot fix  
- When a quick fix is needed for production, create a branch off of `master` branch with the hotfix/ prefix, like so: `hotfix/<issue-number><hotfix name>`  
- Create a pull request from hotfix branch to `master` branch  
- When pull request has been reviewed - merge it, this will push fix to production  
- Create and merge a pull request from hotfix branch to `develop` branch, this will update staging  
- Delete hotfix branch
