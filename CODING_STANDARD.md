# CuraMap Project - Coding Standards  

Welcome to the CuraMap Project! To ensure our codebase is clean, consistent, and easy to work with, we’ve established these coding standards. *Please follow these guidelines carefully.*  

---

## **1. General Coding Principles**  

### **Why Standards Matter**:  
- Makes the codebase easier to read and understand for everyone.  
- Reduces bugs and errors by following proven practices.  
- Helps new team members quickly adapt.  

### **Key Principles**:  
- *Keep it simple*: Write straightforward and clear code.  
- *Don’t Repeat Yourself (DRY)*: Reuse code to avoid duplication.  
- *Modular Design*: Break large tasks into smaller, reusable functions.  
- *Error Handling*: Always anticipate and handle errors gracefully.  

---

## **2. File and Folder Naming Rules**  

### **Folder Names**:  
- Use *kebab-case* for folder names.  
  - Example: `user-authentication`, `admin-dashboard`  

### **File Names**:  
- **JavaScript** files: `camelCase.js`  
  - Example: `userLogin.js`  
- **CSS** files: `kebab-case.css`  
  - Example: `user-login-form.css`  
- **Python** files: `snake_case.py`  
  - Example: `process_data.py`  

---

## **3. Code Formatting**  

### **Indentation**:  
- **JavaScript, HTML, and CSS**: Use 2 spaces for indentation.  
- **Python**: Use 4 spaces for indentation.  

### **Line Length**:  
- Keep lines of code to *80 characters or fewer*. If necessary, break the line.  

### **Spacing**:  
- Add a single blank line between functions and sections of code for readability.  

### **Example (JavaScript)**:  
```javascript
function calculateAge(birthYear) {
  const currentYear = new Date().getFullYear();
  return currentYear - birthYear;
}

console.log(calculateAge(1995));
```

---

## **4. Commenting Guidelines**  

### **Why Comment?**  
- Comments explain what the code does and why it’s written a certain way.  

### **General Rules**:  
- Use comments to explain complex logic or important decisions.  
- Avoid obvious comments (e.g., `i = 0; // set i to 0`).  

### **Comment Syntax**:  

**JavaScript**:  
- Single-line: `// This is a single-line comment`  
- Multi-line:  
```javascript
/*
  This function handles user login validation.
  It checks both username and password.
*/
```

**Python**:  
- Single-line: `# This is a single-line comment`  

**Example (Python)**:  
```python
# Function to calculate average score
def calculate_average(scores):
    # Ensure the list is not empty to avoid division by zero
    if len(scores) == 0:
        return 0
    return sum(scores) / len(scores)
```

---

## **5. Naming Conventions**  

### **Variables and Functions**:  
- Use **camelCase** for JavaScript.  
  - Example: `userName`, `validateForm()`  
- Use **snake_case** for Python.  
  - Example: `user_name`, `validate_form()`  

### **Constants**:  
- Use **UPPER_CASE** for constants.  
  - Example: `MAX_USERS = 100`  

### **Classes**:  
- Use **PascalCase** for class names.  
  - Example: `UserProfile`  

---

## **6. Git Workflow**  

### **Branch Naming**:  
- Use `feature/feature-name` for new features.  
  - Example: `feature/user-authentication`  
- Use `bugfix/issue-name` for bug fixes.  
  - Example: `bugfix/login-error`  

### **Commit Messages**:  
- Write short and clear messages describing the change.  

**Examples**:  
- `Feat: Add user login validation`  
- `Fix: Resolve crash on form submission`  
- `Refactor: Optimize database queries`  

### **Example Workflow**:  
1. Create a new branch for your task:  
   ```bash
   git checkout -b feature/user-authentication
   ```
2. After making changes, stage and commit:  
   ```bash
   git add .
   git commit -m "Feat: Add user authentication"
   ```
3. Push to the remote repository:  
   ```bash
   git push origin feature/user-authentication
   ```
4. Open a Pull Request (PR) for code review.  

---

## **7. Front-End Standards**  

### **HTML**:  
- Use semantic tags: `<header>`, `<section>`, `<footer>`.  
- Include `alt` attributes for images.  

### **CSS**:  
- Follow the BEM (Block Element Modifier) methodology.  
  - Example:  
    ```css
    .form__input--error {
      border: 1px solid red;
    }
    ```

### **JavaScript**:  
- Avoid using `var`. Use `let` or `const`.  
- Prefer arrow functions for short, anonymous functions.  

---

## **8. Back-End Standards**  

### **Error Handling**:  
- Always handle errors using `try-catch` blocks in JavaScript.  
  ```javascript
  try {
    // risky operation
  } catch (error) {
    console.error('An error occurred:', error);
  }
  ```

### **Security**:  
- Never hardcode sensitive information like passwords or API keys.  
- Use environment variables for sensitive data.  

---

## **9. Linting Tools**  

### **Tools We Use**:  
- **JavaScript**: ESLint  
- **Python**: flake8  

### **How to Run Linting**:  
1. Install the required linter:  
   ```bash
   npm install eslint --save-dev
   ```
2. Run the linter:  
   ```bash
   eslint yourfile.js
   ```

---

## **10. Final Checklist Before Committing Code**  

- [ ] Code passes all tests.  
- [ ] Code follows the formatting and naming conventions.  
- [ ] Comments are clear and concise.  
- [ ] No sensitive information is committed.  
- [ ] Run the linter and fix any issues.  

---

By following these standards, we’ll build a clean, efficient, and scalable codebase together. Thank you for your commitment to quality!
