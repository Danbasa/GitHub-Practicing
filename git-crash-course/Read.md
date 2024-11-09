
## Git Hidden Folder

There is a hidden folder called .git, which tells you that your project 
is a git repo.


If we want to create a git repo in a new project, we create the
folder and initialize that repo using `git init`

```sh
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git add .
# make changes to readme.md
git commit -m "add readme file"

```

## Cloning

We can clone three ways: HTTPS. SSH, GitHub CLI

Since we are using GitHub Codespaaces we'll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```sh
git clone https://github.com/Danbasa/GitHub-Practicing.git
cd GitHub-Examples
```

## Commits

When we want to commit code, we write `git commit` which will open up 
the commit edit meesage in the editor of choice.

```sh
git config --global core.editor vim
```

Set the global editor
```sh
git commit
```

```sh
git commit -m "add another exclamation point"
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to Stage changes that will be included in the commit
We can use to all all possible files

```sh
git add Readme.md
git add .
```

## Reset

Reset allows you to move Staged Changes to unstaged
Useful for reverting all files not to be committed

```sh
git add .
git reset
```

## Status

Shows what files will or will not be committed

```sh
git status
```

## Git config file

Stores your local configurations for git such as email, name, editor, and more.

```sh
git config --show-origin
```

## Log

git log will show recent git commits to the git tree

```sh
git log
```

## Push

When waiting to push a repo to our remote origin

```sh
git push
```