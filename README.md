# Building-management-system
smart-building

# git command 
The daily loop
bash
git status             # what changed?
git add .              # stage everything
git add filename.js    # stage one file
git commit -m "msg"    # save the snapshot
git push               # upload to GitHub
git pull               # download latest from GitHub
Branches (working with a team)
bash
git branch                        # see all branches
git checkout -b feature/login     # create + switch to new branch
git checkout main                 # switch back to main
git merge feature/login           # merge branch into current
git branch -d feature/login       # delete branch after merge
Checking history
bash
git log --oneline                 # short commit history
git log --author="name"           # your commits only
git diff                          # see unstaged changes
git diff HEAD                     # see all changes since last commit
Oops — fixing mistakes
bash
# undo staged file (before commit)
git restore --staged filename.js

# undo changes to a file (before commit)
git restore filename.js

# undo last commit (keeps your changes)
git reset --soft HEAD~1

# undo last commit (deletes your changes) ⚠️
git reset --hard HEAD~1

# fix last commit message
git commit --amend -m "correct message"
Working with GitHub
bash
git remote -v                     # see connected remote
git push origin main              # push to main branch
git push origin feature/login     # push a specific branch
git pull origin main              # pull latest main
Everyday workflow for your BMS team:
bash
# start of day
git pull                          # get latest code

# during work
git status                        # check what changed
git add .                         # stage changes
git commit -m "feat: add login"   # commit

# end of day
git push                          # upload to GitHub
Commit message rules:
feat:     new feature
fix:      bug fix
docs:     readme, comments
style:    formatting only
refactor: restructure code
chore:    deps, config












