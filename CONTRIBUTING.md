# 🧑‍💻 Contributing to SingNRG Projects

Welcome to the team! This guide explains how to work on SingNRG codebases responsibly and consistently.

---

## 🔄 Git Workflow

1. **Clone the repository**  
   ```
   git clone git@github.com:singnrg/project-name.git
   cd project-name
   ```

2. **Create a new branch**  
   Name your branch based on the task:  
   ```
   git checkout -b feature/email-verifier-ui
   ```

3. **Commit often, write clear messages**  
   Use this format:
   ```
   feat: added login form  
   fix: handled null values in webhook  
   docs: updated readme  
   ```

4. **Push your changes**  
   ```
   git push origin feature/email-verifier-ui
   ```

5. **Open a pull request (PR)**  
   - Assign it to your team lead or reviewer
   - Add a short description of what was done

---

## 🧹 Coding Standards

- Use meaningful names for variables, functions, and branches  
- Leave comments where logic may not be obvious  
- Avoid committing `.env`, secrets, or credentials  
- Stick to our stack conventions:  
  - **React + Tailwind** on the front end  
  - **Python FastAPI** or **Node.js** on the back end  
  - Keep code modular and reusable

---

## 🔐 Security & Compliance

- Never hardcode secrets. Use `.env` files.  
- If handling user data, always use HTTPS and follow basic security practices  
- Obey license terms if using external libraries  

---

## 📞 Who to Ask

- For questions on this repo: ask your assigned tech lead  
- For infrastructure/devops issues: ask Nick or the system administrator  
- For new project proposals: submit a request in the `#dev-ideas` channel on Teams

---

Thank you for keeping our code clean, fast, and production-ready.
