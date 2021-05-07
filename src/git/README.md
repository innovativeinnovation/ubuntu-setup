# Git

[Git](https://git-scm.com/) is a version-control system for tracking changes
in computer files and coordinating work on those files among multiple people.

## Installation

```bash
sudo apt install git
```

## Configuration

Every git user should first introduce himself to git, by running these
two commands:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

We can see all of the configuration items that have been set by typing:

```bash
git config --list
```

## Usage

Create a new repository:

```bash
git init
```

Checkout a repository:

```bash
git clone /path/to/repository                 # local
git clone username@host:/path/to/repository   # remote
```

Add and commit:

```bash
git add <filename>
git add *
git commit -m "Commit message"
```

Status:

```bash
git status
```

Pushing changes:

```bash
git push origin master
```

Update local:

```bash
git pull
```

## Diff with meld

To use meld as difftool, add to your `~/.gitconfig`:

```text
[diff]
    tool = meld
[difftool]
    prompt = false
[difftool "meld"]
    cmd = meld "$LOCAL" "$REMOTE"
```

Use `git difftool` in exactly the same way as you use `git diff`:

```bash
git difftool --dir-diff HEAD .
git difftool --dir-diff master fea-branch
```

## Create a global `.gitignore`

You can create a global `.gitignore` file, which is a list of rules for
ignoring files in every Git repository on your computer.

GitHub maintains an official list of recommended `.gitignore` files for many
popular operating systems, environments, and languages:

```bash
curl https://raw.githubusercontent.com/github/gitignore/master/Global/Linux.gitignore -o ~/.gitignore
```
