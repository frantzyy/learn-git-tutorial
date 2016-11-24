# Lesson 3 - Creating a branch

In this lesson you'll learn to create a branch, add a change to that branch, commit and push the remote sever.


## Step 1 - Show branches in your working directory (local)

`git branch`

## Step 2 - Show all branches, remote and local

`git branch -a`


## Step 3 - Create a new branch

`git branch feature/{yourLastName}`

`git branch -a`

You should see:
* master
feature/yourLastName


## Step 2 - Checkout the new branch

`git checkout feature/{yourLastName}`

`git status`

You should see:
On branch feature/yourLastName
nothing to commit, working directory clean


## Step 3 - Make an update

- in the file you created in the previous lesson (yourName.txt)
- add the following text on line 2: "Comfort level with git before this tutorial: [1-5]"
- add your own rating, 1 being the lowest comfort level, 5 being the highest comfort level.

## Step 4 - Add your updates

`git add -A`

## Step 5 - Commit your updates

`git commit -m "a decriptive message"`

## Step 6 - Check the status

`git status`

## Step 7 - Push your changes

`git push origin feature/{yourLastName}`

## Step 8 - Check the status

`git status`

## Step 9 - Checout master 

`git checkout master`

Notice now your directory has updated and you should see your updates are no longer there. That's because we haven't merged them from your feature branch to the master branch yet.

Juut to prove your changes haven't been lost, checout your feature branch.

`git checkout feature/{yourLastName}`

Now you should see your updates again. Ahh... sigh of relief. 

Take a break now, we'll get into merging your feature back to master next.




