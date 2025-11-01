# GitHub — basics & workflows

This file summarises key GitHub concepts, repository sections, and recommended README contents.

## What is GitHub?

GitHub is a cloud-based hosting service for Git repositories. It provides collaboration features such as issues, pull requests, actions, projects, and more.

## Required fields when creating a repository

1. Repository name (title)
2. Visibility: public or private

## Main repository sections

1. Code
2. Issues
3. Pull requests
4. Actions
5. Projects
6. Wiki
7. Security
8. Insights
9. Settings

## What should be in a README

A good README is descriptive and instructive. Recommended sections:

- Title and short description
- Technology and purpose (why)
- Installation / usage (how to run)
- Features and architecture
- Table of contents (for long docs)
- Motivation and challenges
- Use cases
- Contribution guidelines

## GitHub features & notes

- Files and directories: you can create/edit files directly in the UI; directories are created by including the path when adding a file.
- Branch rules: require PRs, approvals, restrict push/merge — configure in Branch protection rules.
- Personal Access Token (PAT): used as credentials in place of passwords for CLI access since 2021.

## Pull Requests (PR)

Typical PR workflow:

1. Create a branch for your change.
2. Push branch and open a PR targeting the destination branch.
3. Add a clear title and description, link related issues.
4. Request reviewers and address comments.
5. Merge after passing checks and approvals.

PR reviews can include comments on specific lines, approvals, or requests for changes.

## Issues

- Assign people with `@username`.
- Reference issues using `#<number>`.
- Use labels, milestones, and projects to organize work.

## Roles & permissions

- Read: view and discuss
- Triage: manage issues and PRs
- Write: push code
- Maintain: manage repository without sensitive settings
- Admin: full control

## Notes

- For organization SSO and 2FA enforcement, members who haven't enabled 2FA can be removed; ensure organization policies are communicated.
