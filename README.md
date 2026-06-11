# 🎓 Onboarding & Workflow Practice Repository

This repository serves as a practical, hands-on learning environment for mastering **Git workflows**, **Jira collaboration**, **n8n automation engineering**, and **AI-driven integrations**. 

It contains modules that range from basic n8n configurations (Webhooks, HTTP requests, JavaScript nodes) to advanced AI agents interacting with external databases and APIs.

---

## 📖 Table of Contents
1. [Project Folder Structure](#-project-folder-structure)
2. [Git Workflow Guidelines](#-git-workflow-guidelines)
3. [Jira Collaboration Best Practices](#-jira-collaboration-best-practices)
4. [Learning Modules Overview](#-learning-modules-overview)

---

## 📂 Project Folder Structure

```text
onboarding-practice/
├── ai-n8n-workflow/        # AI Customer Support Agent (n8n + OpenRouter AI)
├── ai-sheets-workflow/     # Customer Support Bot integrated with Google Sheets logging
├── n8n-workflows/          # Core n8n learning workflows (HTTP, Webhook, JS)
├── profile.md              # Developer profile page
└── README.md               # Master documentation (this file)
```

---

## 🌿 Git Workflow Guidelines

To maintain code quality and historical clarity, we follow a strict branching and commit convention.

### 1. Branching Strategy
- **`main`**: The stable production branch. Never commit directly to `main`.
- **`feature/branch-name`**: Created for developing new features.
- **`bugfix/issue-description`**: Created for resolving bugs.

*Example command to start a new feature:*
```bash
git checkout -b feature/JIRA-123-add-cart-logic
```

### 2. Commit Message Convention
Commit messages must be clear, descriptive, and prefixed with the type of work and corresponding Jira Ticket Key:
- `feat(JIRA-KEY): description` — for new features.
- `fix(JIRA-KEY): description` — for bug fixes.
- `chore(JIRA-KEY): description` — for build tasks, documentation, or dependency updates.

*Example commit:*
```bash
git commit -m "feat(KAN-5): implement slide-out cart sidebar"
```

### 3. Pull Request (PR) Lifecycle
1. Push your branch to the origin: `git push origin feature/your-branch`.
2. Open a Pull Request on GitHub targeting the `main` branch.
3. Reference the Jira ticket ID in the PR description.
4. Ensure all automated tests/lints pass before requesting reviews from team members.

---

## 💼 Jira Collaboration Best Practices

This workspace is closely bound to our Jira Boards. Keep the following practices in mind:
- **Link Commit & PRs:** By including the Jira ticket ID (e.g., `KAN-12`, `PROJ-7`) in your Git commits and Pull Requests, Jira will automatically link the code activity directly to the corresponding Jira card.
- **Update Statuses Promptly:** When you begin working on a card, transition it from **To Do** to **In Progress**. When submitting a PR, transition it to **In Review**.

---

## 🏫 Learning Modules Overview

### 1. [AI n8n Customer Bot](file:///Users/muhammadsoban/.gemini/antigravity-ide/scratch/onboarding-practice/ai-n8n-workflow)
- **Tech:** n8n, OpenRouter API (OpenAI/Claude), HTML Test Client
- **Goal:** Learn how to design webhook-triggered AI routing, parse natural language queries, and return structured text responses.

### 2. [Google Sheets AI logger](file:///Users/muhammadsoban/.gemini/antigravity-ide/scratch/onboarding-practice/ai-sheets-workflow)
- **Tech:** n8n, Google Sheets API, OpenRouter API
- **Goal:** Learn how to authenticate and read/write values dynamically to spreadsheets from an n8n workflow based on customer requests.

### 3. [Fundamental n8n Workflows](file:///Users/muhammadsoban/.gemini/antigravity-ide/scratch/onboarding-practice/n8n-workflows)
- **Tech:** n8n HTTP Request node, Webhook trigger node, JS Code Execution node
- **Goal:** Learn the foundational blocks of data manipulation, API consumption, custom script mapping, and webhook parsing.
