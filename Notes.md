# 26 June 2024 Git Basics

### Preparing for group meeting presentation on Git Basics
- Local git stuff
    - git init
    - git config --list
        - git config stuff
        - git branch -m main
            - Renames master branch to main
    - git status
    - git add
    - git commit, git commit -m "msg"
    - git log
    - git diff mars.txt
        - for a file/files with uncommitted/unadded(unstaged) changes
    - git diff --staged (shows changes in staging area (added files))
    - git commit (opens default editor so you can write a longer commit message)
    - HEAD is the name of the current version. HEAD~1 is one commit ago. HEAD~2 is two commits ago. Instead of HEAD~2 you can use the git hash which appears in the git log.
    - git diff HEAD~1
    - git checkout HEAD mars.txt
        - checkout HEAD = revert to the version in HEAD, i.e., undoes the unstaged changes. can also do checkout HEAD~1 which will revert to the previous commit.
        - checkout also can switch branches.
    - git show
        - Basically shows the information for the current commit, including the commit message.
    - git revert <hash>
        - Reverts to a previous commit using a commit hash. Requires working tree to be clean (no modifications from the HEAD commit)
        - just doing git revert HEAD basically undoes the most recent commit.

- GitHub stuff, remote repository
    - Setting up SSH keys
        - ssh-keygen -t ed25519 -C "your emaill here"
        - Copy the public key in ~/.ssh
        - Go to github, add that ssh key.
    - Initialize a new online repo. Follow the directions for pushing an existing repo from the command line.
        - From HTTPS or SSH select SSH (thats why we set up SSH keys to begin with)
    - git push, git pull. git fetch
    