# Git commands


## “pull request” a specific commit

Create a new branch with just that change:

```bash
$ git fetch --all
$ git checkout -b my-single-change upstream/master
$ git cherry-pick b50b2e7
$ git push -u origin my-single-change
```

Then create the PR from that branch.

The above assumes you've set up upstream as a remote. If not, do this first:

```bash
git remote add upstream https://github.com/user/repo.git
```

Source: https://stackoverflow.com/a/34027874

## New repository

```
cd git-reps
mkdir wiki
git init wiki

cd wiki
git remote add origin https://github.com/tripl3a/wiki.git
git pull origin master
```

## Add stuff

```
# commit all changes:  
git commit -a
# Push the changes in your local repository to GitHub:
git push origin master
```

## Remove stuff

```
# unversion a file
git rm --cached <filename>
```

## Configure SSH (for GitLab.com)

1.) generate a new key-pair:

```
ssh-keygen -t rsa -C "triple_a@mailbox.org" -P "" -q -f ~/.ssh/gitlab_rsa
```

2.) propagate the new key

```
eval $(ssh-agent -s)
ssh-add ~/.ssh/gitlab_rsa
```

3.) edit .ssh/config

```
# GitLab.com
Host gitlab.com
  Preferredauthentications publickey
  IdentityFile ~/.ssh/gitlab_rsa
```

4.) test setup

```
ssh -T git@gitlab.com
```
5.) clone repo

```
git clone git@gitlab.com:tripl3a/transfer-learning-for-hatespeech-detection.git
```
