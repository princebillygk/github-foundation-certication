# Git features that standout git from other VCS / SCM

- Distributed (stored in both client and servers)

# What is working tree

A set of nested directories that contain the projects that's being worked on

# What is repo

The root directory located at the top of working tree

# Important commands related to git

1. Create a new repository with the folder name "my_project":
    
    ```bash
    git init my_project
    ```
    
2. Add an existing project to a new repository:
    
    ```bash
    cd existing_project
    git init
    ```
    

# The commit structure

1. Commit - meta data - author, log message, commit time
2. Tree - Tracks the names and locations of files and directories in the repo
3. Blob - Binary large object,

# What is hash in Git?

1. A 40 character (160bit) string composed of hexadecimal characters (0-9, a-f)
2. Pseudedo random number generate hash function

# `git log`

Shows newest to oldest commits - space to see more, q to quit

1. git log -n : Show last n commits
2. git log `file-name`: Show commits that modified the specified file
3. git log --since='Month day year': Shows commits since the specified date
4. git log --until='Month day year': Shows commits until the specified date
5. We can also combine --since and --until to show commits in a specific date range
6. We can also provide natural language dates like --since='2 weeks ago', '15 July 2024'
7. Recommended format 'YYYY-MM-DD'
8. We cannot other characters in data format such as ','
9. `git log --oneline` shows one line commit

# `git show <commit-hash>`

10. We can use only the first 8-10 characters of the commit hash
11. Shows both commit message and changes as diff
12. git diff --staged : Compares staged changes with the last commit
13. Compare 2 commits: git diff : Recent commit should be second
14. `HEAD` : Points to the latest commit on the current branch
15. `HEAD~n` : Points to the nth commit before HEAD
16. see diff of a specific file in a specific commit: git diff

# Git Branches

## General

- Multiple people can work on the same project simulataniously
- Compare state
- Each branch should have a specific purpose

```shell
git branch #list all local branches
git switch <branch-name> # switch to a different branch
git branch speed-test # create a new branch but not switch
git switch -c speed-test # create a new branch and switch to it
```

## Compare and modify

```shell
git diff main summary-statistics # compare two branches
git branch -m curr_branch new_name # change branch name
git branch -d branch_name # Delete a branch
git branch -D umerged_branch_name # Delete a unmerged branch
```

# Merge

**Source**: the branch we want to merge from  
**destination**: the branch we want to merge into

## Method 1

```shell
# Move to the destination branch
git switch destination_branch
# Merge
git merge source_branch
```

## Method 2

```shell
git merge source_branch destination_branch
```

## Merge Conflicts

- Prevention is better than cure. Rather avoid editing the same file in multiple branches to avoid merge conflict

# Remotes

- Computer breaks down or loose it we can use a different computer to get our code
- Copying code to multiple remotes
- When cloning git will automatically name the remote origin

```shell
git clone path-to-project-repo # clone a repo with same name
git clone path-to-repo new_repo_name # clone a repo with name
git remote # get remotes
git remote -v # get remote with urls
git remote add name url # add a new repo

git fetch origin # fetch all branch from the remote to local repo
git fetch origin branch_name # fetch only one branch
git merge origin # if we don't mention any branch name the main branch will be merged

# fetch ad merge in single command
git pull origin dev # do both git fetch and merge together

git push remote local_branch # push local_branch to remote
```

# `.git-keep`

`.git-keep` a empty file that is used track empty folder by git

# Abbreviations

|Short Form|Meaning|
|---|---|
|VSC|Version Control System|
|SCM|Software Configuration management|
