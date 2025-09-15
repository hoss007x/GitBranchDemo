# Hello World

# Workflows

Standard commit process
 edit file(s) -> add to stage -> commit

## Commands
```
git init                    # Creates the repo
git add <filename>          # Add to the stage
git commit -m "msg"         # Commits with MSG
git commit -A               # Commits All files
git log                     # list of commits
git branch                  # List of Branches
git checkout -b <branch>    # Creates and checkout
git checkout <branch>       # Checkout target branch
git status                  # Im Lost, i need an adult
git pull origin <branch>    # Pulls latest code
git merge <targetBranch>    # merge target branch into current branch
```

## Actively Using Commands
```
git status
git checkout <branch>
git pull origin <branch>
git add -A
git commit -m "msg"
git checkout <branch>
git merge <to branch> <from branch>
git push origin <from branch>
git tag -a v1.0.0 -m "derp!"
```

## Git Flow Explinations
```
1. **Stage all changes**:
   - `git add -A`
   - This stages all modified and new files in the repository.

2. **Commit changes**:
   - `git commit -m "Finalized UI with CLR and DEL buttons"`
   - Replace "msg" with a descriptive message. Here, I used a message reflecting the current state.

3. **Switch to main branch** (interpreting `git checkout`):
   - `git checkout main`
   - This switches to the `main` branch to prepare for merging. If you meant a different branch, specify it (e.g., `git checkout <branch-name>`).

4. **Merge the UI branch** (interpreting `git merge`):
   - `git merge ui-branch`
   - This merges the `ui-branch` into `main`. Resolve any conflicts if they arise.

5. **Push to remote repository**:
   - `git push origin main`
   - Replace `<branch>` with `main` since we're merging into `main`. If you want to push the `ui-branch` instead, use `git push origin ui-branch`.

6. **Tag the release**:
   - `git tag -a v1.0.0 -m "derp!"`
   - This creates an annotated tag `v1.0.0` with the message "derp!". Push the tag with `git push origin v1.0.0` if needed.
```