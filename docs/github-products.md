# GitHub products & security (summary)

This document summarises common GitHub products, billing notes, and security-related items relevant to the certification.

## Products & plans (high level)

- GitHub Free — individuals and small projects (public/private repos with limits on some features)
- GitHub Pro — advanced individual features
- GitHub Team — collaboration features for teams
- GitHub Enterprise — organization-grade security, SSO, audit logs, and advanced controls

Billing can be subscription-based (seats) and usage-based (Actions minutes, Packages, Codespaces).

## GitHub Actions & Packages

- Actions: CI/CD workflows. Minutes and usage may be billed depending on plan.
- Packages: Package registry (npm, Docker, etc.) with billing/limits depending on plan.

## Security features

- Dependabot: automated dependency updates and alerts
- Code scanning (CodeQL): static analysis for vulnerabilities
- Secrets scanning: detect credentials in commits
- Security policy (SECURITY.md): tell users how to report issues

## Removing sensitive data

- `git filter-repo` — flexible and recommended for rewriting history
- `BFG Repo-Cleaner` — faster, simpler tool for common cases

## Codespaces / github.dev

- Codespaces: cloud dev environment with `.devcontainer` configuration
- `github.dev`: quick browser-based editor for small edits
