# Lesson 2 - Git basics

In this lesson you'll go through the basics of cloning a repo, adding a new file, commiting it, and pushing back the remote server.

# Step 1 - Clone a repo

TODO: add aws insprof-learn-git repo here

`git clone blah blah`

# Step 2 - Add a new file

- create a new file
- name it {lastName}_{firstName}.txt
- add your email to it

# Step 3 - Add new file to staging directory

`git add nameOfFile.txt` 

This will add all the files you've created to your staging directory. This is similar to checking in your files to a change set in RTC.

Alternatively, if you have a lot of changes and want to add them all you can do:

`git add --all` or `git add -A` or `git .`

# Step 4 - Commit the new file

`commit -m "a descriptive messages"`


# Step 5 - Check the status

`git status`


# Step 6 - Push changes to origin

`git push origin master`

How do you know what to push to? Well by doing a `git status` prior, git tells you what branch you are currently working on and in the normal flow you will want to push to that branch's remote origin first. Later on we'll get in to merging branches.

# Step 7 - Check the status

`git status`

You should see this:

```
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
```