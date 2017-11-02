#GIT COMMANDS:

## Reset local repository branch to master:
git fetch origin
git reset --hard origin/master
git checkout master

## Init Repo:

init: git init
add all: git add -A
commit all: git commit -am „commit message“
rename last commit: git commit --amend

## Ticket bearbeiten:
switch to branch: git checkout „feature_branch“
create and switch to branch: git checkout -b „feature_branch“
show remote branches: git branch -r
To delete a local branch: git branch -d feature_branch
To delete a remote branch: git push origin :feature_branch
To show remote branches: git remote show origin

## Ticket auf Master rebase:
git checkout „master“
git pull
git checkout „feature_branch“
git rebase master
git checkout master
git merge - - ff-only feature_branch

## Tags:
LÖSCHEN:
git tag -d 12345
git push origin :12345
NEU ANLEGEN
git tag 12345
To push a single tag:
git push origin <tag_name>
And the following command should push all tags (not recommended):
git push --tags

## Wenn man zu alten kommt zurück will:
(optional) seine Änderungen backupen auf neuen branch git checkout -b 
git reset --hard 378b312 (wo 378b312 die SH1 eines anderen commits spezieller: tag/branch/commit id)
—> http://stackoverflow.com/questions/1616957/how-do-you-roll-back-reset-a-git-repository-to-a-particular-commit

to update remote branches (clean up the deleted ones): 
git remote update origin --prune

to find all branches that belong to me, use the script:
find-my-branches.sh mniemczyk

to revert a commit:

git revert e793a613a06aeacac2d784616b849bca0b8f9a95 (if last thats the most upper commit)

## mvn version

mvn versions:set -DnewVersion=1.1.22

# GIT HUB

git remote set-url origin ssh://git@git.vendor.com:7999/java/cloudportal.git

Git rarere feature enable: git config --global rerere.enabled true
more about: https://git-scm.com/blog/2010/03/08/rerere.html

1. Fork their repo on Github
	2. In your local, add a new remote to your fork; then fetch it, and push your changes up to it
	
	    git remote add my-fork git@github...my-fork.git
	    git fetch my-fork
	    git push my-fork


I.
echo "# notes" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/Macilias/notes.git
git push -u origin master

II.
git remote add origin https://github.com/Macilias/notes.git
git push -u origin master
