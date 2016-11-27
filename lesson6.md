# Lesson 6 - Merging a branch with conflicts

In this lesson we'll make changes to your file from a feature branch and the master to mimic a conflict. Then show you how to resolve it.

## Step 1 - Create a new branch

`git branch feature/lastName2`

`git checkout feature/lastName2`

Note: a shortcut for these steps is:

`git checkout -b feature/lastName2`


## Step 2 - Update your file

On line 3, update your file with `Changed in feature branch`


## Step 3 - Add, commit, and push changes 

`git add --all`

`git commit -m "adding an update from feature branch"`

`git push origin feature/lastName2`

## Step 4 - Checkout out master and make some changes

`git checkout master`

On line 3, update your file with `Changed in master branch`

`git add --all`

`git commit -m "adding an update from master"`

`git push origin master`

## Step 5 - Attempt to merge feature branch

`git status`

Confirm you are on master.

`git merge feature/lastName2`

You should get an error with the following:
```
Auto-merging teams/appfolder/lastName_firstName.txt
CONFLICT (content): Merge conflict in teams/appfolder/lastName_firstName.txt
Automatic merge failed; fix conflicts and then commit the result.
```

## Step 6 - Open your editor for the file

You should see comments added to the file that indicate what changed and where the conflict is:

```
<<<<<<< HEAD
Changed in master
=======
Changed in feature branch

>>>>>>> feature/frantz-mergeWithError
```

This is where you would decide if you need keep master, keep what's in the feature, or combination of both.

Update your file how you wish.

## step 7 - Add, commit, push to master.

Do as we normally do and now you'll have all your changes in master.



