# Git — core concepts & commands

This file contains concise Git fundamentals and practical command references useful for revision and exam prep.

## Core concepts

- Working tree: The local directory structure where you edit files.
- Repository (repo): The top-level directory that stores the Git history and metadata.
- Commit: A snapshot of the repository; includes metadata (author, message, timestamp).
- Tree / Blob: Internal Git objects; trees track directories, blobs store file contents.
- SHA-1 hash: Git object identifiers (40 hex characters). You can usually use the first 8–10 characters.

## Common commands

- Initialize a new repo:

```bash
git init my_project
```

- Add an existing project to Git:

```bash
cd existing_project
git init
```

- View log (newest → oldest):

```bash
git log --oneline
git log -n 5           # last 5 commits
git log --since=2024-07-01 --until=2024-07-31
```

- Show commit and diff:

```bash
git show <commit-hash>
```

- Diff staged changes vs last commit:

```bash
git diff --staged
```

## Reverting and restoring

- Revert a commit (creates a new commit that undoes the changes):

```bash
git revert <commit>
git revert HEAD        # revert last commit
git revert --no-edit <commit>
```

- Restore files from a specific commit (does not create a commit by itself):

```bash
git checkout HEAD~1 -- path/to/file
```

- Unstage a file (keep changes in working directory):

```bash
git restore --staged <file>
```

## Branches & merging

- Create and switch branches:

```bash
git branch feature-x        # create
git switch feature-x        # switch
git switch -c feature-x     # create + switch
```

- Merge into current branch:

```bash
# switch to target branch first
git switch main
git merge feature-x
```

- Delete branches:

```bash
git branch -d branch_name    # delete (safe)
git branch -D branch_name    # force delete unmerged
```

## Remotes

- Clone a repository:

```bash
git clone <url>
git clone <url> new_name
```

- Remote operations:

```bash
git remote -v
git remote add origin <url>
git fetch origin
git pull origin main
git push origin feature-x
```

## Notes

- `.gitkeep` is a convention: an empty file used to keep otherwise-empty directories in Git.
- Abbreviations: VCS = Version Control System, SCM = Software Configuration Management.

