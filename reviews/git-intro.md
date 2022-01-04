# Review 1/4/22 - Git Intro

## Command Line

`cd <filepath>` change directories
`mkdir <folder>` make directory
`echo <text> > <filepath>` write text to a file (file is created if not exists)
`touch <file>` create a file (linux/unix only)
`.` current directory
`..` parent directory
`mv`, `move` to move a file/folder from the old location to the new
`rm`, `remove` to remove a file
`rm -rf <folder>`, `rmdir -R <folder>` to remove a folder with contents
`open`, `start` to open a file (all files have a default application)
`ls`, `dir` to list items in a directory
`head <file>` displays the first 10 lines of a file (can be changed to be more than 10)
`tail <file>` displays the last 10 lines of a file (can be changed to be more than 10)

## Git

Linus Torvalds is seen as the creator of Git in 2005.

Git is a _distributed version control system_.

`git status` receive feedback with git tracking a folder (e.g. current branch, untracked files, modified files, staged files, unpushed commits, etc)
`git init` initializes an empty git repository
`git fetch` downloads latest updates from the remote repo
`git merge` merges latest updates from a fetch to the local project
`git pull` _fetches and merges_ the latest updates in a remote repository
`git log` displays previous commits
`git diff` displays the current _changes_ (_uncommitted_) from the previously (_latest_) committed version
`git remote -v` list remote branches for this repo

All files _to be ignored_ by Git, should be listed in a `.gitignore` file

### Git Workflow

`git add <filepath>` adds file(s) to the staging area (can use `.` to add all modified files to the staging area)
`git commit -m "description"` equilivent to a "save"; takes a _snapshot_ of the current project/files at the current version
`git push --set-upstream origin main` to push to github (for the first time) and set the main branch as upstream
`git push` to push to github on the set upstream
