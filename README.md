BASIC COMMANDS
git log
- show all the commit history
- main branch





making a new branch:
git checkout -b new-branch
git push -u origin new-branch


what does -b and -u do?x

Yes, you're correct! git commit -am combines two operations:

-a (or --all): Automatically stages all modified and deleted files that are already tracked by Git
-m: Allows you to specify the commit message inline
So git commit -am "message" is equivalent to:
git add -u  # stages all modified/deleted tracked files
git commit -m "message"
Important notes:

It only affects tracked files - it won't add new/untracked files to the commit
It stages modified and deleted files - but not new files you've created
It's a shortcut - saves you from having to run git add separately for changes to existing files
# Instead of:
git add file1.txt file2.txt  # (for modified files)
git commit -m "Update files"

# You can do:
git commit -am "Update files"

If you have new files that aren't tracked yet, you'll still need to git add them first, or use git add . to stage everything including new files.




BRANCH:
tanline of commits

what you could do is make a different branch
a branch is like a movable pointer that points to a commit in history


master is the main branch
we call it main
push to main


why should we make branches
- isolation: test stuff before deploying it, work independently in branches
- parallel is where you merge the features
- organization
- stability

git branch:
- shows all the branches in the repo
- git checkout <branch_name>   
    - git checkout <feature-1> creates a new feature branch, if you commit it commits to the branch and then

- git checkout -b <branch_name> creates a new branch and switches to it

- git merge <branch_name>

git branch -d <branch-name>





merge conflicts:









pull request
- a requestr to merge your code into another branch usually main
-    gi

