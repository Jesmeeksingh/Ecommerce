# 🧠 Git Cheat Sheet for This Project

This file is your quick-reference guide to using Git safely and effectively in this project.

---

## 🌱 1. Creating a New Branch

```bash
# From main branch
git checkout main
git pull origin main

# Create a new branch
git checkout -b feature/your-feature-name
```

✅ Use branch naming patterns:
- `feature/` for new features (e.g. `feature/login-ui`)
- `bugfix/` for bug fixes (e.g. `bugfix/cart-totals`)
- `refactor/` for code refactors
- `docs/` for documentation updates

---

## 💾 2. Committing Changes

```bash
git add .
git commit -m "Your message explaining what you changed"
```

✏️ Write meaningful commit messages:
- Bad: "Update"
- Good: "Fix incorrect cart price calculation"

---

## 🚀 3. Pushing Your Branch to GitHub

```bash
git push origin feature/your-feature-name
```

---

## 🔁 4. Creating a Pull Request (PR)

1. Go to your repo on GitHub.
2. Switch to your branch.
3. Click **“Compare & pull request”**.
4. Fill in the PR title and description.
5. Click **“Create pull request”**.

---

## 🔀 5. Merging the PR

After review or testing:

- Click **“Merge pull request”**
- Then click **“Confirm merge”**
- Finally, click **“Delete branch”**

---

## 🔄 6. Sync Your Local `main` Branch

```bash
git checkout main
git pull origin main
```

---

## 💥 7. Undoing Mistakes (Safely)

```bash
# Undo the last commit but keep the changes
git reset --soft HEAD~1

# Discard uncommitted changes
git checkout -- .

# See what changed before commit
git status
git diff
```

---

## 🧪 8. Checking Branches

```bash
git branch        # See local branches
git branch -r     # See remote branches
git checkout -b branch-name origin/branch-name  # Track a remote branch
```

---

## 🔍 9. Useful Tips

- Never push directly to `main`.
- Always work on feature branches.
- Always pull the latest `main` before creating a new branch.
- Use pull requests for all merges — even for solo work!

---

📝 Last updated: Auto-generated
