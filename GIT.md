# Git
## Git commands
- Clone remote repository to local
  `git clone <remote repo url>`

- Retrieve the remote resources to local
  `git pull`
- Stage the local changes
  `git add .`  (stage all local changes)
  `git add <individual file>` (stage an individual resource)

- Unstage the local changes
  `git restore --staged <resource name>` 
  `git reset <resource name>`

- Submit the local changes
  `git commit -m "commit messages" `
- Send local changes to remote
  `git push`

- Check the local repository status
  `git status`
- Check the changes or difference of the resources
  `git diff` (display all changes)
  `git diff <individual resource>` (display the changes of the individual resource)
- Discard the local changes
  `git checkout -- .` (discard all local changes)
  `git checkout -- <individual resource>` (discard the changes of the individual resource)

- Check the local branches
  `git branch`
- Check the remote branches
  `git branch -r`
- Check all branches (local & remote branches)
  `git branch -a`
- Create a new branch and switch to the new branch
  `git checkout -b <new branch name>`
- Switch to another branch
  `git checkout <branch name>`
- Delete a local branch
  `git branch -D <local branch name>`

- Push local branch to remote
  `git push -u origin <local branch name>`

## Pull Request on Remote
- On remote, create pull request to merge development branch to main branch
  - create pull request: `base: main-branch`, `compare: developer's branch`
  - if there is conflict, then resolve the conflict first
  - after resolving the conflict, commit the merge
  - (optional) delete developer's branch