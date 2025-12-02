# **ALX Advanced Git – GitFlow Project**

This project introduces the Git-Flow branching model and demonstrates how to structure features, releases, and hotfixes in a professional development workflow. You will initialize Git-Flow, create feature and release branches, resolve merges, implement Git hooks, and prepare the repository for manual review.

---

## 🚀 **Project Overview**

Git-Flow is a branching strategy that organizes development into clearly defined phases:

* **main** – production-ready code
* **develop** – integration branch for ongoing work
* **feature/*** – isolated development of new features
* **release/*** – preparation for stable releases
* **hotfix/*** – rapid fixes for urgent production issues

This workflow helps maintain clean, stable code while supporting collaborative development.

---

## 🎯 **Learning Objectives**

By completing this project, you will be able to:

* Understand the structure and purpose of Git-Flow.
* Manage feature development, releases, and hotfixes using Git.
* Apply Git-Flow commands to real-world collaborative scenarios.
* Use Git hooks for automation.
* Tag and maintain production-ready releases.

---

## 🧩 **Tasks Summary**

### **0. Setting up GitFlow**

* Install Git-Flow
* Create repository `ALXprodev-advanced_git`
* Create and push `develop` branch
* Initialize Git-Flow with default settings
* Add and push `README.md`

### **1. Creating a Feature Branch**

* Create `feature/implement-login` from `develop`
* Add `login-page/README.md` containing:
  **"Login Feature Coming soon"**
* Commit with message:
  `feat: scaffolding login page`
* Push to remote

### **2. Creating a Release Branch**

* Create `feature/implement-signup`
* Add `signup-page/README.md` with text:
  **"feature coming soon"**
* Merge feature branches into `develop`
* Create `release/1.0.0`
* Update signup page with:
  **"data requirements: email, firstName, lastName, profilePic"**
* Merge release into both `main` and `develop`
* Tag release as `v1.0.0` and push tags

### **3. Git Hooks and Automation**

Implement:

* **pre-commit hook** — ensures every directory has a `README.md`
* **post-merge hook** — logs merges into `main`

---

## 🛠️ **Common Git-Flow Commands**

```bash
git flow init -d                 # Initialize Git-Flow
git flow feature start <name>    # Start feature branch
git flow feature finish <name>   # Finish feature
git flow release start <x.x.x>   # Start release branch
git flow release finish <x.x.x>  # Finish release and tag
git flow hotfix start <x.x.x>    # Start hotfix
git flow hotfix finish <x.x.x>   # Finish hotfix
```

---

## 📌 **Git Hooks Used in This Project**

### **pre-commit**

Validates that each project directory contains a README.

### **post-merge**

Appends merge information into `.git/merge.log`.

> Git hooks live inside `.git/hooks/` and must be executable.

---

## 🧪 **Assessment Requirements**

To receive full credit:

* Complete all tasks
* Push all branches to GitHub
* Tag the final release
* Ensure Git hooks are functional
* Generate and submit review link before deadline
* Pass the automated presence checks

---

## 📂 **Repository Structure**

```
ALXprodev-advanced_git/
│
├── login-page/
│   └── README.md
│
├── signup-page/
│   └── README.md
│
├── .git/
│   ├── hooks/
│   │   ├── pre-commit
│   │   └── post-merge
│
└── README.md   ← this file
```

---
