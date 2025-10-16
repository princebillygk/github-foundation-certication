# Important commands related to git
1) Create a new repository with the folder name "my_project":
   ```bash
   git init my_project
   ```
2) Add an existing project to a new repository:
   ```bash
   cd existing_project
   git init
   ```


# The commit structure
1) Commit - meta data - author, log message, commit time
2) Tree - Tracks the names and locations of files and directories in the repo
3) Blob - Binary large object,


# What is hash in Git?
1) A 40 character string composed of hexadecimal characters (0-9, a-f)
2) Pseudedo random number generate hash function 

# `git log`
Shows newest to oldest commits - space to see more, q to quit
1) - <n>: Show last n commits
2) git log `file-name`: Show commits that modified the specified file
3) git log --since='Month day year': Shows commits since the specified date
4) git log --until='Month day year': Shows commits until the specified date
5) We can also combine --since and --until to show commits in a specific date range 
6) We can also provide natural language dates like --since='2 weeks ago', '15 July 2024'
7) Recommended format 'YYYY-MM-DD'
8) We cannot other characters in data format such as ','

# `git show <commit-hash>` 
1) We can use only the first 8-10 characters of the commit hash
2) Shows both commit message and changes as diff
3) git diff --staged : Compares staged changes with the last commit
4) Compare 2 commits: git diff <commit-hash-1> <commit-hash-2> : Recent commit should be second
4) `HEAD` : Points to the latest commit on the current branch
5) `HEAD~n` : Points to the nth commit before HEAD
6) see diff of a specific file in a specific commit: git diff <file-name> 
