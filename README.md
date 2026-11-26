# Git & GitHub Collaboration Workshop

A collaborative directory of developers learning Git and GitHub through a
hands-on contribution workflow.

## What is this project?

This repository is a practical learning space. Contributors use it to practise
version control, branching, commits, forks, issues, pull requests, code review,
and automated checks.

The exercise is deliberately simple: each participant adds a personal Markdown
profile in the `contributors/` directory. Each person works in a separate file,
so the group can practise parallel contributions without intentionally editing
the same lines.

## Learning goals

By contributing, you will practise how to:

- Create and clone Git repositories.
- Inspect, stage, commit, and push changes.
- Work on a feature branch instead of committing task work to `main`.
- Understand the difference between `origin` and `upstream`.
- Fork a repository and synchronise your fork.
- Track work with GitHub Issues.
- Submit a Pull Request (PR) for review.
- Read basic CI checks from GitHub Actions.

## Quick start

1. Fork this repository on GitHub.
2. Clone **your fork** to your computer.
3. Add the original repository as the `upstream` remote.
4. Read [`CONTRIBUTING.md`](CONTRIBUTING.md).
5. Pick up your assigned issue and create a feature branch.
6. Add your profile using [`contributors/template.md`](contributors/template.md).
7. Push your branch and open a PR to the original repository's `main` branch.

The full project context is in [`docs/PROJECT_OVERVIEW.md`](docs/PROJECT_OVERVIEW.md).

## Repository layout

```text
.
├── README.md
├── CONTRIBUTING.md
├── .gitignore
├── docs/
│   └── PROJECT_OVERVIEW.md
├── contributors/
│   └── template.md
└── .github/
    ├── ISSUE_TEMPLATE/
    ├── PULL_REQUEST_TEMPLATE.md
    └── workflows/
```

## Important links

- [Contribution guide](CONTRIBUTING.md)
- [Project overview](docs/PROJECT_OVERVIEW.md)
- [Contributor profile template](contributors/template.md)
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

## Workshop rule

**One contributor, one profile file, one feature branch, one Pull Request.**

Do not commit your task directly to `main`. Follow the contribution guide and
ask questions in your issue or Pull Request if you get stuck.
