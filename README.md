# AI Test Commander

**AI Test Commander** is an AI-driven test automation framework designed to minimize manual QA efforts by orchestrating modular software testing agents using artificial intelligence.

This system empowers a single QA Manager to oversee all test operations — from UI and API tests to database validation — while AI agents autonomously execute tasks, analyze results, and report back.

---

## 🚀 Project Vision

- **Fully autonomous QA pipeline** driven by intelligent agents
- **Commander-Soldier architecture** for scalable and modular control
- Support for **UI**, **API**, **Database**, and future test domains (e.g., Security, Performance)
- Replace large QA teams with a single QA Manager supervising AI-driven agents
- Integrate with modern CI/CD pipelines and reduce time-to-release

---

## 🧠 Architecture Overview

### 🧠 Commander Agent
Acts as the test orchestrator. It:
- Assigns tasks to soldier agents
- Collects and analyzes their results
- Generates test reports
- Notifies QA Manager for approval or feedback
- Updates test plans based on feedback loops

### 🛡️ Soldier Agents
Independent AI agents that perform specific test responsibilities:
- **UI Agent**: Automates frontend end-to-end flows
- **API Agent**: Validates REST and SOAP services
- **DB Agent**: Performs data integrity and schema validation
- (Future): `AuthAgent`, `PerformanceAgent`, `SecurityAgent`, etc.

---

## 📦 Directory Structure

ai-test-commander/
├── commander/ # Central brain (Commander agent)
├── agents/
│ ├── ui/ # UI testing agent
│ └── api/ # API testing agent
├── prompts/ # Prompt templates for agent conversations
├── config/ # Environment and test configs
├── utils/ # Helper modules
├── logs/ # Execution logs
├── README.md
├── requirements.txt
└── .gitignore


---

## 🔧 Technologies Used

| Area            | Stack                                |
|-----------------|--------------------------------------|
| Language        | Python 3.x                           |
| AI / LLM        | OpenAI GPT API, LangChain            |
| Web Framework   | FastAPI                              |
| Testing         | Pytest, HTTPX                        |
| Infra/Tools     | Git, GitHub, VS Code                 |
| Planned         | Docker, Redis, GitHub Actions        |

---

## 📊 Key Features (MVP Scope)

- [x] Modular agent system (UI, API, DB)
- [x] Configurable agent prompt templates
- [x] Commander-agent task distribution logic
- [x] Local development environment with GitHub integration
- [ ] LLM result interpretation module
- [ ] CI/CD integration with feedback loop
- [ ] Dashboard for test reports and heatmaps

---

## 📅 Development Timeline

| Phase | Status     | Notes |
|-------|------------|-------|
| Day 1 | ✅ Complete | Project goals and scope defined |
| Day 2 | ✅ Complete | System architecture finalized |
| Day 3 | ✅ Complete | GitHub setup, folder structure |
| Day 4 | 🔜          | Python venv, requirements setup |
| Day 5+| 🔜          | Agent logic development |

📌 Current Status: v1.0.0 (MVP phase under development – core agent architecture being built)

📌 Version Roadmap
This project follows a structured versioning strategy, where each version milestone reflects a significant advancement in product capability, stability, and scalability.

🔷 v1.0.0 – MVP (Minimum Viable Product)
The first complete working version focused on AI-powered modular test execution.

Commander Agent architecture implemented

Basic UI & API test agents functional

Prompt-based agent communication enabled

Test output generation (basic format)

Manual setup via requirements.txt

GitHub version control and modular codebase in place

🔷 v2.0.0 – Smart Agents + Developer Experience
Enhanced intelligence, flexibility, and developer tooling improvements.

Smarter soldier agents (multi-step reasoning, retries, feedback loop)

.env-based config for secrets and environment variables

Switch from requirements.txt to pyproject.toml + Poetry

Dockerfile support for simplified environment setup

JSON-formatted structured test results

CLI or minimal web dashboard (optional)

🔷 v3.0.0 – Production Readiness + Scalability
From demo to product. Built for real-world integration and enterprise use.

Full CI/CD integration (GitHub Actions)

Real-time test dashboard & report visualizations

Plugin-based agent extensibility

Async agent orchestration

Multi-environment testing support (prod/stage/test)

User auth, multi-project handling (if needed for B2B)

This roadmap ensures the project evolves from a test automation concept into a scalable, AI-driven test infrastructure ready for enterprise adoption.

---

## 🧪 How to Set Up (Local)

```bash
# Clone the repo
git clone https://github.com/kiziltasbaris10/ai-test-commander.git
cd ai-test-commander

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate (on Windows)

# Install dependencies
pip install -r requirements.txt

