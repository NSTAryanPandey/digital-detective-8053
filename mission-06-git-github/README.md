# Mission 6: Git Branching and GitHub

## 1. Mission Title
Git Branching and Pull Requests

## 2. Task/Objective
Practise creating a new Git branch, making commits on it, pushing it to GitHub, opening a pull request, and merging the changes back into `main`.

## 3. Work Completed
- Created a new branch called `mission6-branch` using `git checkout -b`.
- Made an edit and committed it directly on that branch.
- Pushed the branch up to GitHub with `git push -u origin mission6-branch`.
- Opened a pull request from `mission6-branch` into `main` on GitHub.
- Merged the pull request on GitHub.
- Switched back to `main` locally and pulled down the merged changes.

## 4. Commands/Tools Used
`git checkout -b mission6-branch`, `git add`, `git commit`, `git push -u origin mission6-branch`, `git checkout main`, `git pull`

## 5. My Understanding
Basically, a branch is just a separate line of work inside the repository that doesn't touch `main` until you merge it. Developers use branches so they can build new features or test fixes without accidentally breaking the main working code. A pull request (PR) is a way to ask for your branch's changes to be reviewed and merged into another branch. Merging through a PR is useful because it lets you or your teammates double-check the changes and catch issues before anything goes into `main`.

## 6. Difficulties Faced
At first, I wasn't sure if working on a new branch meant I had to open a separate terminal window or folder. I kept checking my branch status so I wouldn't accidentally commit straight to `main`.

## 7. How I Resolved Them
I ran `git branch` and `git status` before committing, which showed the `*` next to `mission6-branch` and confirmed Git switches branches right inside the same folder and terminal window.

## 8. Evidence/Files
Pull Request #1 on GitHub: "Add mission 6 branch work" (merged into `main`). is this good?