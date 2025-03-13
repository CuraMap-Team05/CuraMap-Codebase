# **Contributing to CuraMap**

Thank you for your interest in contributing to the CuraMap Project! Whether you're fixing a bug, adding a new feature, or improving documentation, we’re excited to have you on board. This guide will walk you through the process of contributing to our project.

---

### **Table of Contents**
1. [Code of Conduct](#CODE_OF_CONDUCT.md)  
2. [Getting Started](#getting-started)  
3. [Branching Workflow](#BRANCHING.md)  
4. [Coding Standards](#CODING_STANDARD.md)  
5. [Pull Request Guidelines](#PULL_REQUEST_TEMPLATE.md)  
6. [Useful Links](#useful-links)  

---

### **1. Code of Conduct**

Please read and adhere to our [Code of Conduct](CODE_OF_CONDUCT.md). We expect all contributors to maintain a respectful and welcoming environment.

---

### **2. Getting Started**

#### **Fork the Repository**  
1. Navigate to the project repository on GitHub.  
2. Click the *Fork* button at the top right.  
3. Clone the forked repository to your local machine:  
   ```bash
   git clone git@github.com:CuraMap-Team05/CuraMap-Codebase.git
   ```

#### **Setting Up Your Local Environment**

1. Navigate to the project directory:  
   ```bash
   cd CuraMap
   ```
2. Install dependencies (if any):  
   ```bash
   npm install  # For JavaScript projects
   ```

#### **Synchronizing Your Fork**

To keep your fork up to date with the development repository:  
```bash
git remote add upstream git@github.com:CuraMap-Team05/CuraMap-Codebase.git
git fetch upstream
git merge upstream/development
```

---

### **3. Branching Workflow**

We follow the Git Feature Branch Workflow. Here’s how to contribute:

1. **Create a new branch for your task**:  
   ```bash
   git checkout -b feature/your-feature-name
   ```
2. **Make your changes and commit them**:  
   ```bash
   git add .
   git commit -m "Feat: Add new feature"
   ```
3. **Push your branch to GitHub**:  
   ```bash
   git push origin feature/your-feature-name
   ```

For detailed guidelines, check our Branching Workflow Guide.

---

### **4. Coding Standards**

All contributors must follow our Coding Standards. This ensures a consistent and clean codebase.

#### **Key Highlights**:
- Use meaningful variable names.  
- Follow proper indentation and spacing.  
- Write clear and concise comments.  

Refer to the full document [here](#CODING_STANDARD.md).

---

### **5. Pull Request Guidelines**

Once your work is ready, submit a Pull Request (PR):

1. Go to the **Pull Requests** tab on GitHub.  
2. Click **New Pull Request**.  
3. Select your feature branch and compare it to `main`.  
4. Provide a clear title and description for your PR.  

For detailed steps, check our Pull Request Template [here](#PULL_REQUEST_TEMPLATE.md).

---

### **6. Useful Links**

Here are some important resources to guide your contributions:  
- [Code of Conduct](#CODE_OF_CONDUCT.md)  
- [Branching Workflow Guide](#BRANCHING.md)  
- [Coding Standards](#CODING_STANDARD.md)  
- [Pull Request Template](#PULL_REQUEST_TEMPLATE.md)  

---

### **Need Help?**

If you encounter any issues or have questions, feel free to open an issue or contact the project maintainers. We’re here to help!
               
---

Thank you for contributing to CuraMap! Let’s build something amazing together. 
