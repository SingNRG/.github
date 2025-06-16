# 🧪 Developer Setup Guide – SingNRG Internal

This guide walks you through setting up your local development environment to work on SingNRG tools.

---

## 🛠 Prerequisites

Make sure you have the following installed:

- **Git** – https://git-scm.com  
- **Node.js (v18+)** – https://nodejs.org  
- **Python (3.10+)** – https://www.python.org  
- **Docker** – https://www.docker.com  
- **PostgreSQL** (or use Supabase CLI if the project uses Supabase)

We recommend VSCode and WSL2 (for Windows users).

---

## 🧬 Project Setup

1. **Clone the repo**
   ```bash
   git clone git@github.com:singnrg/project-name.git
   cd project-name
   ```

2. **Install dependencies**

   If it's a **Node.js project**:
   ```bash
   npm install
   ```

   If it's a **Python backend**:
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. **Environment variables**

   Copy the example env file and fill in values:
   ```bash
   cp .env.example .env
   ```

   You may need API keys for:
   - OpenAI
   - Supabase
   - Stripe/AppSumo
   - Mailgun, Brevo, etc.

   These will be shared securely via Teams.

4. **Run the app locally**

   - For full-stack apps:
     ```bash
     docker-compose up
     ```

   - For frontend-only:
     ```bash
     npm run dev
     ```

   - For backend-only:
     ```bash
     uvicorn main:app --reload
     ```

---

## 💾 Database Access

Some projects use Supabase (hosted) or local PostgreSQL.

- Credentials will be provided for dev/staging
- Do not make schema changes unless instructed
- Use migrations if needed (e.g. Alembic, Prisma, etc.)

---

## 🚀 Deployment Notes

- Most deployments are via **Vercel** (frontend) or **Lightsail** (backend)  
- DO NOT deploy directly — submit a request to Nick or the team lead  
- Use Git branches (`dev`, `staging`, `main`) properly to avoid breaking production

---

## 🧠 Tips

- Use ChatGPT, Copilot, and other AI tools — smart use is encouraged  
- Comment and document your work as you go  
- Clean, modular code > clever, complex code

---

Need help? Ask on Teams or tag your lead.

Happy shipping! 🚀
