# CherryPick – Git Workflow Simulation (DevOps Focus)

This repository is a **hands-on Git mini project** created to practice and demonstrate
real-world **DevOps Git workflows**, focusing on branch management, cherry-picking,
and history reconciliation.

Unlike basic Git demos, this project intentionally simulates **failure scenarios**
and recovery workflows commonly encountered in production environments.

🎯 Project Objective

- Understand how **cherry-pick** is used to selectively promote fixes
- Work with **divergent branch histories**
- Handle **non–fast-forward push rejections**
- Compare **merge vs rebase** decisions
- Visualize and maintain a **clean, traceable commit history**

🌿 Branch Strategy Used

| Branch | Purpose |
|------|--------|
| `main` | Primary integration branch |
| `master` | Simulated production branch |
| `dev` | Development/testing changes |
| `hotfix/*` | Emergency production fixes |

🔧 Git Concepts Practiced

- Cherry-pick across branches
- Non–fast-forward push rejection handling
- Merge vs rebase decision making
- Reset, revert, and checkout recovery
- Tagging important commits
- Commit history visualization using graphs

🧪 Simulated Scenarios

✔ Cherry-picking specific commits from `dev` to `master`  
✔ Handling push rejection due to divergent histories  
✔ Resolving branch mismatch between `main` and `master`  
✔ Tagging stable commits for release tracking  
✔ Visual inspection using `git log --graph`

📜 Key Commands Used

```bash
git cherry-pick <commit-id>
git log --oneline --graph --all
git push origin main
git pull --rebase origin main
git tag latest-commit
