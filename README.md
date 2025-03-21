# 📚 Horus Project – Contribution Guide

Welcome to the Horus AI Infrastructure project!  
To maintain **clarity**, **collaboration**, and **code quality**, this repository follows strict contribution norms and task management rules. Please read this carefully before pushing anything to the project.

---

## ✅ Git Commit Convention Cheat Sheet

Every commit must follow this format:

```
[SYMBOL] Title

Full description of what was done, why it was done, and how (if needed).
```

### 🔣 Symbols & Their Meanings

| Symbol | Meaning                               | Use when...                                                                 |
|--------|----------------------------------------|------------------------------------------------------------------------------|
| `[+]`  | **Add**                                | You’re adding a new file, feature, class, or functionality.                 |
| `[~]`  | **Update / Modify / Refactor**         | You’ve updated, improved, or refactored existing code.                      |
| `[x]`  | **Fix**                                | You’re fixing a bug, error, typo, or issue.                                 |
| `[-]`  | **Remove**                             | You’ve deleted code, removed files, or deprecated features.                 |
| `[!]`  | **Important / Breaking change**        | You’re introducing something critical, like a breaking change or hotfix.   |
| `[#]`  | **Docs / Comment**                     | You’ve updated documentation, comments, or README files.                    |
| `[>]`  | **Performance / Optimization**         | You’ve improved speed, memory usage, or system efficiency.                 |
| `[?]`  | **Work In Progress (WIP)**             | You’re committing unfinished work or an experimental prototype.             |

### 🧠 Description Guidelines

- Use **present tense** in titles (e.g., "Add login feature")
- Be short and clear in the title
- Provide context in the description

**Example:**

```
[+] Add multi-agent orchestrator for Horus

Implemented a new Python orchestrator module to manage inter-agent
communication via RPC. Enables real-time task delegation and supports
plug-and-play agents.
```

---

## 📌 Task & Issue Tracking Cheat Sheet

All work must be associated with a GitHub **Issue**. No issue = no code.

### 🛠️ Task Rules

1. **Create a GitHub Issue** before you start any task.
2. **Create a Branch from that Issue** using:
   ```
   issue-<issue-number>-<short-description>
   ```
   _Example: `issue-42-agent-routing`_
3. **Assign yourself** to the issue.
4. **Estimate time** required (e.g., `2h`, `1d`, `3d`).
5. **Work only in that branch**, and reference the issue in your commits and PRs.
6. **Open a Pull Request**, link the issue with:
   ```
   Fixes #<issue-number>
   ```
7. **Get 2 reviewers from the group who DID NOT write the code**.
8. **Only merge after 2 approvals.**
9. **Use Squash & Merge**, then delete the branch.
10. **Issue closes automatically** if `Fixes #` is used, else close it manually.

### 📋 Example Issue Template

```
Title: [Core] Implement communication handler

Description:
Create a core handler that routes messages between AI agents using internal protocol.

Estimate: 1d  
Assignee: @yourusername  
Labels: enhancement, AI  
Milestone: MVP v1  
```

### 🧪 Commit Example

```
[+] Add core message router between AI agents

Implements inter-agent communication via internal event bus.
Fixes #42
```

---

## 🔁 Summary

| 📌 Rule | Description |
|--------|-------------|
| 🔧 Task → Issue | All work begins as an issue |
| 🌿 Branch per Issue | Name format: `issue-<id>-<desc>` |
| 📤 Commits | Follow commit symbol rules |
| 📂 Pull Requests | Linked to issue, must be reviewed |
| ✅ Merge Rules | 2 non-authors must approve |
| 🧹 After Merge | Use "Squash and Merge", delete branch |

---

By following these rules, we ensure a professional and maintainable codebase that’s easy for new contributors to join and follow.  
Let’s build Horus the right way. 💡
