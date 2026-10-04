# git-cli-practic
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
