��# darkearth

Workflow:

For merge conflicts (especially if it's just the projectsettings.asset file):

git checkout --theirs the-merge-error-file-name

Then re-add the files and commit the changes. You should then be merged!

Updating your repo from master:

git checkout master
git pull origin master
git checkout your-branch-name
git merge master

When you're committing something (still on your own branch):

git add .
git commit -m description-of-commit-here
git push origin your-branch-name

Then go to github and create a pull request between your branch and master. Before pushing, you may want to use git status to make sure that the right files were added to your commit

If there are changes in your repo that you didn't do yourself or want to discard, enter

git checkout -- .

To create a new branch, use git checkout -b new-branch-name

To see what branch you're on, use git branch

To switch to a branch, use git checkout your-branch-name
