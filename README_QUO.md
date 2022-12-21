# How do I update or sync a forked repository on GitHub?
https://stackoverflow.com/questions/7244321/how-do-i-update-or-sync-a-forked-repository-on-github

## Add the remote, call it "upstream":

git remote add upstream https://github.com/opening-hours/opening_hours.js.git

## Fetch all the branches of that remote into remote-tracking branches

git fetch upstream

## Make sure that you're on your master branch:

git checkout master

## Rewrite your master branch so that any commits of yours that aren't already in upstream/master are replayed on top of that other branch:

git rebase upstream/master

# Publish to npm

make check-holidays

npm run build

npm login

npm publish