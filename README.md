# hello-github


Hi Human,

What are u doing?

It might be a good idea to have an environment that is automatically updated to the master branch. Only, in this case, the name of this environment might differ from the branch name. Suppose you have a staging environment, a pre-production environment, and a production environment. In this case, deploy the master branch to staging. To deploy to pre-production, create a merge request from the master branch to the pre-production branch. Go live by merging the pre-production branch into the production branch. This workflow, where commits only flow downstream, ensures that everything is tested in all environments. If you need to cherry-pick a commit with a hotfix, it is common to develop it on a feature branch and merge it into master with a merge request. In this case, do not delete the feature branch yet. If master passes automatic testing, you then merge the feature branch into the other branches. If this is not possible because more manual testing is required, you can send merge requests from the feature branch to the downstream branches.
