# Lesson 5 - Deleting a branch


## Step 1 - Confirm you are not in the feature branch you wish to delete

`git status`

You should be on master, if not:

`git checkout master`


## Step 2 - Delete your feature branch

`git branch -d feature/yourLastName`

Git will confirm your branch has been deleted

## Step 3 - Display all branches

`git branch -a`

You will see your branch is no longer listed locally, but it's still there remotely.

## Step 4 - Delete your remote branch

`git push origin --delete feature/yourLastName`

That's it now, you've completed your first feature!


