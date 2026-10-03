# 🤖 AI Testing Platform

> **AI-powered full-stack software testing platform** for generating test cases, tracking test runs, and building an intelligent QA workflow.

## 🖥️ Dashboard Preview

> 📸 **Add your dashboard screenshot here**
>
> Put your image at:
>
> `screenshots/dashboard.png`

![AI Testing Platform Dashboard](./screenshots/dashboard.png)

---

## ✨ Features

- 🤖 **AI Test Case Generator**
- 🧪 Test case management
- ▶️ Test execution tracking
- 📊 Testing overview dashboard
- 📈 Pass / fail statistics
- 🧠 LLM-powered test scenario generation
- ⚡ FastAPI REST API
- ⚛️ React.js frontend
- 🗄️ Database-backed test history
- 📱 Responsive dashboard
- 🔌 Automation-ready architecture

---

## 🏗️ Architecture

```text
┌──────────────────────────────┐
│       React Frontend         │
│   Dashboard / AI Generator   │
└──────────────┬───────────────┘
               │ REST API
               ▼
┌──────────────────────────────┐
│       FastAPI Backend        │
│  Tests / AI / Statistics     │
└──────────────┬───────────────┘
               │
       ┌───────┴────────┐
       ▼                ▼
┌─────────────┐  ┌──────────────┐
│  Database   │  │     LLM      │
│   SQLite    │  │ OpenAI-ready │
└─────────────┘  └──────────────┘
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React.js |
| Build Tool | Vite |
| Backend | Python + FastAPI |
| AI / LLM | OpenAI API |
| Database | SQLite |
| ORM | SQLAlchemy |
| API | REST |
| Testing | Pytest-ready |
| Automation | Playwright-ready |

---

## 📂 Project Structure

```text
AI-Testing-Platform/
│
├── backend/
│   ├── app/
│   │   ├── ai_service.py
│   │   ├── database.py
│   │   ├── main.py
│   │   ├── models.py
│   │   ├── routes.py
│   │   └── schemas.py
│   ├── tests/
│   ├── requirements.txt
│   └── .env.example
│
├── frontend/
│   ├── src/
│   │   ├── main.jsx
│   │   └── style.css
│   ├── package.json
│   └── index.html
│
├── screenshots/
│   └── dashboard.png
│
├── .gitignore
└── README.md
```

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/basukumar56258-cpu/AI-Testing-Platform.git
cd AI-Testing-Platform
```

### 2. Start Backend

```bash
cd backend
python -m venv venv
```

#### Windows

```bash
venv\Scripts\activate
```

#### macOS / Linux

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create `.env` from `.env.example`.

Start FastAPI:

```bash
uvicorn app.main:app --reload
```

Backend:

```text
http://127.0.0.1:8000
```

API documentation:

```text
http://127.0.0.1:8000/docs
```

---

### 3. Start Frontend

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

Open:

```text
http://localhost:5173
```

---

## 🧠 AI Test Case Generator

Enter a feature such as:

```text
User login with email, password,
forgot password and account lockout
```

The AI can generate scenarios covering:

- ✅ Positive cases
- ❌ Negative cases
- 🔍 Validation cases
- 📏 Boundary cases
- ⚠️ Error handling
- 🔐 Security-related scenarios

Without an API key, the project runs with a local demo generator. Add your LLM API key to `.env` for live generation.

---

## 🔐 Environment Variables

Create:

```text
backend/.env
```

Example:

```env
DATABASE_URL=sqlite:///./ai_testing.db
OPENAI_API_KEY=your_api_key_here
OPENAI_MODEL=gpt-4o-mini
```

**Never commit your real API key to GitHub.**

---

## 📊 Dashboard

The dashboard provides:

- Total test runs
- Passed tests
- Failed tests
- Pass rate
- Recent execution history
- AI-generated test scenarios

---

## 🧪 API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/health` | API health |
| GET | `/api/stats` | Testing statistics |
| GET | `/api/tests` | Test history |
| POST | `/api/tests` | Create test run |
| DELETE | `/api/tests/{id}` | Delete test |
| POST | `/api/ai/generate` | Generate AI test cases |

---

## 🔮 Future Roadmap

- [ ] Playwright browser automation
- [ ] Selenium integration
- [ ] Postman collection execution
- [ ] Real-time test execution
- [ ] JWT authentication
- [ ] MySQL / PostgreSQL support
- [ ] RAG-based QA knowledge base
- [ ] AI bug analysis
- [ ] AI-generated automation scripts
- [ ] CI/CD integration
- [ ] Docker deployment
- [ ] Test report export

---

## 👨‍💻 Author

**Basu Kumar**

GitHub:  
https://github.com/basukumar56258-cpu

---

## ⭐ Support

If this project helps you, consider giving the repository a ⭐ on GitHub.
