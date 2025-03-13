
# **Contributing Guidelines for CuraMap**

Welcome to the CuraMap Project! This document will guide you on how to contribute effectively. Follow these steps to ensure we maintain a clean, organized, and efficient workflow.

---

## **1. Understanding Our Branching Workflow**

Our repository uses a branching strategy to manage changes systematically. Here’s a breakdown of the key branches:

### **Main Branches**
- **`main`**: This is the stable, production-ready branch.
  - Contains only tested and approved code.
  - **Do not** make any changes directly to this branch.

- **`development`**: This is the active development branch.
  - All new features and updates should be merged here before moving to `main`.

### **Feature Branches**
- Feature branches are used to develop new features or work on specific tasks.
- **Naming convention**:  
  ```plaintext
  feature/<feature-name>
  ```
  **Example**: `feature/user-registration`.

---

## **2. Steps for Contributing**

### **Step 1: Fork the Repository**
- Fork this repository to your personal GitHub account.

### **Step 2: Clone the Repository**
- Clone the repository to your local machine:
  ```bash
  git clone git@github.com:CuraMap-Team05/CuraMap-Codebase.git
  ```

### **Step 3: Set Upstream Remote**
- After cloning, set the upstream remote to the main repository:
  ```bash
  cd CuraMap
  git remote add upstream git@github.com:CuraMap-Team05/CuraMap-Codebase.git
  ```

---

## **3. Creating a Feature Branch**

### **Step 1: Pull Latest Changes**
Before creating a branch, ensure your local `development` branch is up-to-date:
```bash
git checkout development
git pull upstream development
```

### **Step 2: Create a New Feature Branch**
Create a feature branch for your task:
```bash
git checkout -b feature/<feature-name>
```
**Example**:
```bash
git checkout -b feature/user-registration
```

---

## **4. Working on Your Feature**

Make your changes in the appropriate files. Follow these steps after completing your task:

### **Step 1: Add and Commit Changes**
- **Stage your changes**:
  ```bash
  git add .
  ```
- **Commit your changes** with a descriptive message:
  ```bash
  git commit -m "Added user registration form"
  ```

---

## **5. Pushing Your Changes**
- Push your feature branch to the remote repository:
  ```bash
  git push origin feature/<feature-name>
  ```
**Example**:
```bash
git push origin feature/user-registration
```

---

## **6. Creating a Pull Request (PR)**

1. Go to the GitHub repository.
2. Select your feature branch.
3. Click the **"Pull Request"** button.
4. Write a clear description of the changes made.
5. Assign the PR to the team lead for review.

---

## **7. Reviewing and Merging Pull Requests**

- Once the PR is reviewed and approved, it will be merged into the `develop` branch.
- After merging, the feature branch will be deleted to keep the repository clean.

---

## **8. Important Notes**

- Always work on a **feature branch**, never directly on `main` or `develop`.
- Keep your commits small and descriptive.
- If you encounter issues, ask for help in the project’s communication channel.

---

## **9. Git Commands Cheat Sheet**

Here’s a quick reference for common Git commands:

- **Clone repository**:
  ```bash
  git clone <repo-url>
  ```

- **Create a new branch**:
  ```bash
  git checkout -b feature/<feature-name>
  ```

- **Switch branches**:
  ```bash
  git checkout <branch-name>
  ```

- **Stage changes**:
  ```bash
  git add .
  ```

- **Commit changes**:
  ```bash
  git commit -m "Your commit message"
  ```

- **Push changes**:
  ```bash
  git push origin <branch-name>
  ```

- **Pull latest changes**:
  ```bash
  git pull upstream development
  ```

---

By following these guidelines, we’ll ensure a smooth and organized development process. Thank you for contributing to CuraMap!
