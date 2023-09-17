# Git

---

## Commands

`git config --global user.name "name"` - setup users name in global config

`git config --global user.email <email>` - setup users email in global config

`git init` - initialization git in project

`git status` - status local files

`git log` - show log of all commits

- `git log --oneline` - short log

- `git log --graph --oneline` - short log with drawled graph

`git diff <(commit-id/branch)-from> <(commit-id/branch)-to>` - show log difference in commits

- `git diff --staged` - show log difference in commits

`git branch <branch-name>` - create branch

- `git branch -v` - info about last commit

- `git branch -M <branch-name>` - rename current branch

- `git branch -d <branch-name>` - deletes this branch

`git checkout <branch-name/commit-id>` - change current (HEAD) branch or change current commit

- `git checkout -b <branch-name>` - create and change current (HEAD) branch

`git add <file1> <file2>` - add files for git indexing

`git commit` - add commit

- `git commit -m "message"` - add commit changes with message

- `git commit -am "message"` - add commit all last changes with message

- `git commit --amend -m "new message"` - rename last changes commit

- `git commit --amend --no-edit` - expand last commit with new files

- `git commit --amend -c <commit-id>` - rename commit by id

`git remote add origin <url>` - connect to first time created repo

- `git remote add pb <url>` - connect to already exist repo

- `git remote -v` - log connected remotes

`git stash` - archive last changes, which not committed (unfinished changes)

- `git stash pop` - get archive changes

`git reset <commit-id>` - return to commit-id

- `git reset --hard` - return to one commit back

`git restore <file>` - restore non staged file

- `git restore --staged <file>` - restore staged file

`git revert <commit-id>` - reverts that commit with a new commit

`git push` - upload last changes

- `git push -u origin <branch-name>` - upload branch

`git pull` - download last changes

## The sequence of actions when connecting to the working repository

1. `git init`

2. `git add .`

3. `git commit -m "Init"`

4. `git branch -M main`

5. `git remote add origin <url>`

6. `git push -u origin main`

## The sequence of actions when connecting to already existing repository

1. `git clone <url>`

2. `cd <cloned-repo-folder>`

3. `git remote add pb <url>`

## Remove [untrack files](https://stackoverflow.com/questions/45400361/why-is-gitignore-not-ignoring-my-files)

1. `git rm -r --cached`

2. `git add .`

3. `git commit -m "Untrack files in .gitignore"`

## Some abbreviations

`-f` or `--force` - force action

`--staged` - staged (prepared with `add` command) files

`~` - parent / home

`@` - HEAD - last commit

`*` or `.` - all; _`*`may not find files whose names begin with `.` (like `.env`)_
