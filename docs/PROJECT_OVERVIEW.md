# Project Overview

## Purpose

The Git & GitHub Collaboration Workshop repository is a small shared project
for practising the contribution workflow used by software teams and open-source
projects.

It is not intended to be a production application. Its value is the workflow:
participants use Git locally, collaborate through GitHub, and see how a change
moves from an issue to a reviewed and merged Pull Request.

## Scope

The workshop focuses on:

- Local version control with Git.
- Repository initialisation and cloning.
- Working trees, staging areas, and commits.
- Branching and merging.
- Fork-based collaboration.
- `origin` and `upstream` remotes.
- Issues, assignees, labels, and acceptance criteria.
- Pull Requests and code review.
- Merge conflict awareness and resolution.
- Commit and branch naming conventions.
- Repository hygiene and `.gitignore`.
- GitHub Actions as an introduction to Continuous Integration.

## The contributor exercise

Each participant creates one Markdown profile in `contributors/`. The profile
must be a new file named after their GitHub username. Contributors should not
edit another participant's file or the shared template.

This task is intentionally small and parallelisable. It allows several people
to practise the same workflow without deliberately competing to modify the
same file.

## Repository layout

| Path | Purpose |
|---|---|
| `README.md` | Project introduction and quick start. |
| `CONTRIBUTING.md` | Contribution workflow and standards. |
| `docs/PROJECT_OVERVIEW.md` | Project purpose, scope, and structure. |
| `contributors/template.md` | Reusable profile structure. |
| `contributors/<username>.md` | One profile per participant. |
| `.github/ISSUE_TEMPLATE/` | Reusable issue template. |
| `.github/PULL_REQUEST_TEMPLATE.md` | Pull Request checklist. |
| `.github/workflows/validate.yml` | Automated Markdown quality check. |
| `.gitignore` | Common local/generated files to exclude. |

## Definition of done

A participant's contribution is complete when:

1. Their profile is added in a separate Markdown file.
2. The change is committed on a descriptively named branch.
3. The branch is pushed to their fork.
4. A PR is opened against the original repository's `main` branch.
5. The PR references the assigned issue.
6. Automated checks pass and the maintainer can review the change.

## Out of scope

This repository does not attempt to teach every advanced Git feature or to
implement a production software service. Commands such as interactive rebase,
submodules, bisect, and reflog are useful follow-up topics, not prerequisites
for completing the workshop.
