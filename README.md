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