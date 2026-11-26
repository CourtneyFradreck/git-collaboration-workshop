# Contributing

Thank you for taking part in the Git & GitHub Collaboration Workshop. This
repository is designed to help contributors practise a realistic, reviewable
workflow.

## Before you start

- Have a GitHub account.
- Install Git and configure your commit identity.
- Make sure you can authenticate to GitHub from your computer.
- Read the issue assigned to you.

## Contribution workflow

### 1. Fork the repository

Use the **Fork** button on GitHub. Your fork is a copy under your own GitHub
account.

### 2. Clone your fork

Replace `YOUR-USERNAME` with your GitHub username:

```bash
git clone https://github.com/YOUR-USERNAME/git-collaboration-workshop.git
cd git-collaboration-workshop
```

### 3. Add the original repository as `upstream`

Replace `ORIGINAL-OWNER` with the account that owns the workshop repository:

```bash
git remote add upstream https://github.com/ORIGINAL-OWNER/git-collaboration-workshop.git
git remote -v
```

`origin` should point to your fork. `upstream` should point to the original
workshop repository.

### 4. Update your local `main`

Before starting a task, bring your local copy of `main` up to date:

```bash
git fetch upstream
git switch main
git merge --ff-only upstream/main
git push origin main
```

The fast-forward-only merge is suitable when your fork's `main` has no separate
commits and is simply behind the original repository. If Git refuses, stop and
inspect the history rather than forcing the operation.

### 5. Create a feature branch

Use a descriptive branch name. For this exercise:

```bash
git switch -c feat/add-YOUR-USERNAME-profile
```

Do not create your contribution directly on `main`.

### 6. Add your profile

Copy the structure in `contributors/template.md` into a new file:

```text
contributors/YOUR-USERNAME.md
```

Replace the placeholders with your own non-sensitive information. Do not edit
the shared template file; create a separate file for your profile.

### 7. Stage, commit, and push

```bash
git status
git add contributors/YOUR-USERNAME.md
git diff --staged
git commit -m "feat: add YOUR-USERNAME profile"
git push -u origin feat/add-YOUR-USERNAME-profile
```

### 8. Open a Pull Request

On GitHub, open a PR with:

- **Base repository:** the original workshop repository.
- **Base branch:** `main`.
- **Head repository:** your fork.
- **Compare branch:** your feature branch.

Use the Pull Request template. Include `Closes #ISSUE_NUMBER` in the
description so the issue can be closed automatically when the PR is merged.

## Branch naming

Use this format:

```text
<type>/<short-description>
```

Examples:

```text
feat/add-courtney-profile
docs/improve-readme
fix/broken-profile-link
chore/update-guidelines
ci/add-markdown-check
```

Use lowercase words separated by hyphens. Keep the name short but meaningful.

## Commit messages

Use the Conventional Commits format:

```text
<type>[optional scope]: <description>
```

Examples:

```text
feat: add contributor profile
docs: update project overview
fix: correct profile link
ci: add Markdown validation
```

## Pull Request expectations

A good PR should:

- Explain what changed and why.
- Link the issue it addresses.
- Be limited to one coherent task.
- Follow the profile template.
- Pass the automated Markdown check.
- Be ready for another person to review.

Do not include passwords, API keys, tokens, private keys, or other secrets in a
profile or commit.

## Keeping your fork current

After the original repository has merged changes, update your fork before
starting another task:

```bash
git switch main
git fetch upstream
git merge --ff-only upstream/main
git push origin main
```

Then create a new feature branch from the updated `main`.
