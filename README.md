# GitTest
Git test project


Basic commands:
---------------

Configure git author:
git config --global user.name "Sam Smith"
git config --global user.email sam@example.com

Proxy:
git config --global http.proxy http://proxyUsername:proxyPassword@proxy.server.com:port
git config --global https.proxy http://proxyUsername:proxyPassword@proxy.server.com:port

Create local repo:
git init

Clone a git project ot local:
git clone /path/to/repository

For a remote server, use:
git clone username@host:/path/to/repository

Add file to staging:
git add <filename>
git add *

Commit changes:
git commit -m "Commit message"

Commit any files you've added with git add, and also commit any files
you've changed since then:
git commit -a

Send changes to the master branch of
your remote repository:
git push origin master

List the files you've changed and those
you still need to add or commit:
git status

If you haven't connected your local
repository to a remote server, add
the server to be able to push to it:
git remote add origin <server>

List all currently configured remote repositories:
git remote -v

Create a new branch and switch to it (master IS THE MAIN BRANCH!):
git checkout -b <branchname>

Switch from one branch to another:
git checkout <branchname>

List all the branches in your repo, and also tell you what branch you're
currently in:
git branch

Delete the feature branch:
git branch -d <branchname>

Push the branch to your remote repository, so others can use it:
git push origin <branchname>

Push all branches to your remote repository:
git push --all origin

Delete a branch on your remote repository:
git push origin :<branchname>

Fetch and merge changes on the remote server to your working directory:
git pull

To merge a different branch into your active branch:
git merge <branchname>

View all the merge conflicts:
git diff

View the conflicts against the base file:
git diff --base <filename>

Preview changes, before merging:
git diff <sourcebranch> <targetbranch>

After you have manually resolved any conflicts, you 
mark the changed file:
git add <filename>

You can use tagging to mark a significant changeset, such as a release:
git tag 1.0.0 <commitID>

CommitId is the leading characters of the changeset ID, up to 10, but must be unique.
Get the ID using:
git log

Push all tags to remote repository:
git push --tags origin

If you mess up, you can replace the changes in your working tree with the
last content in head:
git checkout -- <filename>

Changes already added to the index, as well as new files, will be kept.


Instead, to drop all your local changes and commits, fetch the latest history
from the server and point your local master branch at it, do this:
git fetch origin
git reset --hard origin/master

Search the working directory for foo():
git grep "foo()"

