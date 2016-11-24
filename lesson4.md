# Lesson 4 - Merging a branch with no conflicts


# Step 1 - Confirm you are your feature branch

`git status`


# Step 2 - Checkout the branch you want to combine your code into

In our scenario, we want to combine your feature branch into master.

`git checkout master`


# Step 3 - Merge code into master

`git merge feature/yourLastName`

# Step 4 - Push code to remote repository

`git push origin master`

# Step 5 - Check status

`git status`

You should see:
```
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
```

You've just completed your first feature! 

It's time to clean up after yourself and delete your branch. See how in the next lesson.