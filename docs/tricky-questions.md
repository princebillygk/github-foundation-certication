# Tricky questions & quick Q&A

Quick Q&A style notes useful for revision.

## Organization & roles

- Organization roles include: Owner, Moderator, Security Manager, Member, Billing Manager, Outside Collaborator, App Manager.
- Minimum permission to push directly depends on branch protection; typically Write permission (but may be enforced via branch rules requiring PRs).

## Pull requests & issues

- Draft PR: a PR not yet ready for review.
- Review statuses: Comment, Approve, Request changes.
- Link PRs to issues by mentioning issue numbers or using keywords (`Fixes #<issue>`).

## Projects & automation

- Project layouts: Table, Board, Roadmap.
- Automations: GitHub Actions, GraphQL/API, and built-in project workflows.

## Codespaces & Copilot

- Codespaces config: `.devcontainer/devcontainer.json`.
- Copilot: free for students, teachers and verified OSS maintainers; it does not learn a single developer's private style from your code.

## Code security & review

- `CODEOWNERS`: specifies who must review changes to certain paths/files.
- CodeQL: GitHub's static analysis tool for security scanning.

## Miscellaneous quick facts

- Gists can be cloned and forked; a public Gist cannot be converted to secret.
- Wiki pages can be edited locally via Git.
- Saved replies help standardize common responses.

## Quick reference table

| Feature | Key point |
|---|---|
| Draft PR | Not ready for review |
| CODEOWNERS | Requires review from designated owners |
| Codespaces config | `.devcontainer/devcontainer.json` |
