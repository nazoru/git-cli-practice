# git-cli-practice
A small repository for practicing Git and GitHub workflows.

This project demonstates common Git commands, branching, commits, rebasing, and pull requests.

```bash
git init
git clone https://github.com/nazoru/git-cli-practice.git
git remote -v

### Staging and Commits

```bash
git status
git add <file>
git add .
git commit -m "Commit message"
git log --oneline

```text

### Branching

```bash
git branch
git branch <branch-name>
git switch <branch-name>
git switch -c <branch-name>
git merge <branch-name>

```text

### Remote Repositories
```bash
git remote -v
git remote add origin <repository-url>
git fetch origin
git pull
git push
git push -u origin main
```

- `gitremote -v` - shows the remote repositories connected to the project.
- `git remote add origin` - connects the local repository to a remote repository.
- `git fetch origin`- downloads information about changes from the remote repository without changing your working files.
- `git pull` - fetches remote changes and integrates them into the current branch.
- `git push` - uploads local commits to the remote repository.
- `git push-u origin main` - pushes `main`and establishes `origin/main` as its upstream branch. 

### History and Recovery

```bash
git rebase <branch-name>
git rebase --continue
git rebase --abort
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit>
```

- `git rebase <branch-name>` - reapplies commits on top of another branch.
- `git rebase --continue` - continues a rebasae afterresolving a conflict.
- `git rebase --abort` - cancels a rebase and returns to the previous state.
- `git reset --soft HEAD~1` - moves the branchback one commit while keeping changes staged.
- `git reset --hard HEAD~1` - moves the branch back one commit and discards working-tree changes.
- `git revert <commit>` - creates a new commit that reverses an earlier commit. 

### Pull Request Workflow

```text
1. Create a feature branch.
2. Make changes on the feature branch.
3. Commit the changes.
4. Push the feature branch to GitHub.
5. Open a Pull Request on GitHub.
6. Review the changes.
7. Merge the Pull Request into main.
```

A Pull Request allows changes from one branch to be reviewed before they are merged into another branch.
