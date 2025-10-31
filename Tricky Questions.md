# GitHub Q&A Reference Guide

## Organization & Roles

### Q: What is the role of organization moderators?

**A:** Moderators are organization members who can:

- Block and unblock non-member contributors
- Set interaction limits
- Hide comments in public repositories owned by the organization

### Q: What are the GitHub organization roles?

**A:** The seven organization roles are:

1. Organization Owner
2. Organization Moderator
3. Security Manager
4. Organization Member
5. Billing Manager
6. Outside Collaborator
7. GitHub App Manager

### Q: What is the minimum permission needed to directly push commits to an organization's repository?

**A:** Manage issues and pull requests

### Q: What is GitHub Teams?

**A:** A group of users from the same organization

### Q: What permissions are needed to add/remove organization members to/from a team?

**A:** Team maintainer permissions

---

## Pull Requests & Issues

### Q: What is a draft pull request?

**A:** A pull request that is not ready to be reviewed yet

### Q: What are the code review pull request statuses?

**A:** Three possible statuses:

1. Comment
2. Approve
3. Request Changes

### Q: How can you link a pull request to GitHub issues?

**A:** Two methods:

1. Manually
2. By mentioning the issue with a keyword and number in the pull request description

### Q: What filters are available for issues?

**A:** Six main filters:

1. `is:issue`
2. `state:open` / `state:closed`
3. `assignee`
4. `author`
5. `label`
6. `project`
7. `milestone`

---

## GitHub Projects

### Q: What layouts are available in GitHub project templates?

**A:** Three layout options:

1. Table
2. Board
3. Roadmap

### Q: What are the three options to automate operations in GitHub Projects?

**A:**

1. GitHub Actions
2. GitHub GraphQL API
3. Project Workflows

### Q: What is the easiest way to add automation to your Project?

**A:** Built-in automation

---

## Codespaces & Development

### Q: What configuration file is used to customize Codespaces?

**A:** `.devcontainer/devcontainer.json`

### Q: What are the different lifecycles for GitHub Codespaces?

**A:** Four lifecycle stages:

1. Create
2. Rebuild
3. Stop
4. Delete

### Q: What are some supported IDEs for GitHub Copilot?

**A:**

- Visual Studio Code
- Visual Studio
- Spyder
- Eclipse

---

## GitHub Copilot

### Q: Can GitHub Copilot learn from individual developer's coding style and preferences?

**A:** No, it generates patterns based on public code and cannot learn individual styles

### Q: Who gets GitHub Copilot for free?

**A:**

- Students
- Teachers
- Maintainers of open-source projects

---

## GitHub Enterprise

### Q: What are the deployment options for GitHub Enterprise?

**A:** Two options:

1. **GitHub Enterprise Server**: Self-hosted
2. **GitHub Enterprise Cloud**: GitHub-hosted

---

## Code Security & Review

### Q: What is the CODEOWNERS file?

**A:** A file that defines individuals or teams responsible for code in a repository, requiring their review on pull requests

### Q: What is CodeQL?

**A:** An analysis tool

---

## Discussions & Communication

### Q: How do announcements differ from other types of discussions?

**A:** Announcements are designed for sharing important news and updates and can be highlighted by maintainers for increased visibility

### Q: What is GitHub slash command?

**A:** The quickest way to insert complex markdown

---

## Git Fundamentals

### Q: What is a Git commit?

**A:** A snapshot of a repository in a stable state

### Q: In Git terminology, what is a "remote"?

**A:** A repository that tracks the same project but resides somewhere else

---

## GitHub Actions

### Q: What are the two types of GitHub Actions?

**A:**

1. Container actions
2. JavaScript actions

---

## InnerSource Metrics

### Q: Which metric indicates your InnerSource program is great and improving?

**A:** A dramatic rise in pull requests addressing bugs in software

---

## Team Synchronization

### Q: What installation permissions are needed to configure team synchronization for Azure AD?

**A:** Read all user profiles

---

## Mobile Features

### Q: What features does GitHub Mobile provide for managing notifications?

**A:** A unified inbox for GitHub notifications with filtering and search capabilities

---

## Important Notes & Tips

### Multiple READMEs Priority

When multiple README files exist, the priority order is:

1. `.github` directory
2. Root directory
3. `.docs` directory

### Branch Creation Steps

1. Go to branch dropdown on main repo page
2. Type the new branch name
3. Press Enter

### Gist Features

- ✅ Can clone Gists using `git clone`
- ✅ Can fork Gists
- ❌ Cannot change public Gist to secret

### Wiki Features

- ✅ Can locally edit Git wikis

### Saved Replies

- ✅ Can create, edit, and delete saved replies in GitHub account settings
- ✅ Can reuse them in issues and pull requests for replying to comments

### Discussion Features

Can perform the following actions on discussions:

- Pin discussions
- Transfer to different repositories
- Convert discussions to issues

### Project Synchronization

- ✅ Synchronization between projects and pull requests/issues happens **bidirectionally**

### GitHub Desktop vs GitHub Online

- ✅ GitHub Desktop: Can visualize branch history
- ❌ GitHub Online: Cannot visualize branch history

---

## Quick Reference Summary

|Feature|Key Point|
|---|---|
|Draft PR|Not ready for review|
|CODEOWNERS|Requires code review from designated owners|
|Codespaces Config|`.devcontainer/devcontainer.json`|
|Project Layouts|Table, Board, Roadmap|
|PR Statuses|Comment, Approve, Request Changes|
|Copilot Access|Free for students, teachers, OSS maintainers|