<div align="center">

# Hi, I'm Made Shandy Krisnanda 👋

**Applied AI Engineering · AI & Application Security · Computer Science @ Universitas Indonesia**

I build AI systems that work in production, and I try to break them before someone else does.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/made-shandy-krisnanda-43ba86260)
[![Email](https://img.shields.io/badge/Email-madeshandykrisnanda%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:madeshandykrisnanda@gmail.com)

</div>

## What I focus on

**🤖 Applied AI engineering.** LLM agents, tool calling and retrieval, plus the ML pipelines behind them. I care about the unglamorous part: evaluation sets, reproducible runs, and numbers I can defend.

**🛡️ AI and application security.** How tool-using agents fail under indirect prompt injection, and which defenses still hold when the model is fooled. I work from threat models, use deterministic scoring, and report the limitations alongside the results.

**⚙️ Reliable engineering.** Tests before claims, least-privilege design, secrets kept out of logs, and CI that proves the change works.

## About me

- 🎓 Computer Science undergraduate at **Universitas Indonesia**.
- 💼 Software Development Engineer Intern at **Glair.ai, GDP Labs**, working on connector reliability, authentication flows, regression coverage and production-quality code.
- 🧑‍🏫 Teaching Assistant Coordinator for Computer Organization, Digital Systems Introduction, and Data Structures & Algorithms.
- 🤝 I use coding agents in my daily workflow: scoped prompts, reviewed diffs, rejected bad output, and changes verified with tests before they land.

## Featured projects

### 🛡️ Agent Warden: AI security

**[Agent Warden](https://github.com/azzelll/agent-warden)**: a red-team harness and a four-layer firewall against indirect prompt injection in tool-using LLM agents.

- **104 attacks**: 5 attacker goals × 3 injection vectors × 8 techniques (English and Indonesian, base64, fake system tags, forged conversation turns, impersonation).
- **4 independent defense layers**: spotlighting, an injection scanner, a tool-call policy whose capabilities come only from the user's prompt (with taint tracking), and an output filter.
- **Deterministic scoring** from observable side effects, never an LLM judge, reported with 95% confidence intervals.
- On a real local model (qwen3:8b): **32.7% → 0% attack success** (95% CI 0–4%) with no loss of benign utility. On a worst-case agent that obeys every injected instruction: 99% → 0%. No single layer was enough on its own.
- **Fine-tuned a multilingual injection detector** to replace the regex layer: best recall on attack techniques it never saw in training (81%), where an off-the-shelf English detector catches 7.7% of Indonesian payloads.
- Ships as an **MCP gateway** (`warden-gateway`) that puts the same policy in front of any stdio MCP server. Workshop paper draft included.

### 🔍 gha-sentinel: CI/CD supply-chain security

**[gha-sentinel](https://github.com/azzelll/gha-sentinel)**: a static scanner for GitHub Actions workflows (pwn requests, script injection, risky token permissions) with SARIF output for code scanning.

- **Scanned the 1,000 most-starred GitHub repositories** (10,213 workflows) and **reviewed every critical finding by hand**: the first version was right 1 time in 31. Six false-positive classes were fixed, cutting findings to 2 **without losing the real vulnerability** (not named publicly).
- Showed that **LLM triage is unsafe as a filter**: a local model dismissed the one real vulnerability. Rules informed by manual review did far better.

## Selected projects

| Project | What I built | Core stack |
| --- | --- | --- |
| [Agent Warden](https://github.com/azzelll/agent-warden) | Prompt-injection red-team harness, tool-call firewall and MCP gateway for LLM agents. | TypeScript, Ollama, MCP, Vitest |
| [AIKO: Academic Inbox & Knowledge Organizer](https://github.com/azzelll/academic-inbox-knowledge-organizer) | Discord bot for a class server: each student binds their own SCELE feed for private deadline lists and a daily DM, asks course-material questions answered with page-level citations (hybrid BM25 + embedding retrieval), and the owner gets Gmail watch rules judged by a local LLM plus GitHub worklog drafts. | TypeScript, discord.js, Ollama, RAG, PostgreSQL, Docker |
| [gha-sentinel](https://github.com/azzelll/gha-sentinel) | Static security scanner for GitHub Actions plus a manually reviewed study of the 1,000 most-starred repositories; found a real pwn request. | Python, YAML analysis, SARIF, GitHub API |
| [SRASTA WiFi CSI](https://github.com/azzelll/SRASTA-WiFi-CSI) | WiFi-CSI activity and fall-detection pipeline: TCN-Lite training, INT8 TFLite inference on Raspberry Pi, and Blynk IoT alerts. **GEMASTIK 2026 finalist (IoT).** | Python, TensorFlow Lite, Raspberry Pi, ESP32 |
| [Carda](https://github.com/azzelll/Carda) | Privacy-first Android prototype for on-device fingertip PPG wellness measurements, designed with explicit safety constraints. **GEMASTIK 2026 finalist (Software Development).** | Kotlin, Jetpack Compose, CameraX, TFLite |
| [Environmental AI / Ecometric](https://github.com/azzelll/environmental-ai-project) | Multimodal environmental-quality system for air, water and soil prediction. The broader Ecometric product won **2nd place** at the Pekan RISTEK Mini Hackathon 2025. | FastAPI, Python, ML, Next.js, Firebase |

## Highlights

- 🏆 **GEMASTIK 2026 Finalist, Internet of Things division:** [SRASTA](https://github.com/azzelll/SRASTA-WiFi-CSI), contactless activity and fall detection from WiFi CSI running on a Raspberry Pi.
- 🏆 **GEMASTIK 2026 Finalist, Software Development division:** [Carda](https://github.com/azzelll/Carda), a privacy-first on-device PPG wellness app for Android.
- 🥈 **2nd Place, Pekan RISTEK Mini Hackathon 2025:** shipped Ecometric as a working full-stack MVP in under 48 hours.
- 🥈 **2nd Place, Pekan RISTEK Data Competition 2025:** LightGBM/XGBoost earthquake early-detection system with cross-validation and out-of-fold blending.
- 🏅 **HFLP Awardee 2026.**

## Tech toolbox

**AI & ML**
`LLM agents` `Tool calling` `RAG` `Ollama` `MCP` `scikit-learn` `LightGBM` `XGBoost` `TensorFlow` `TFLite` `MLflow`

**Security**
`Threat modeling` `Prompt-injection red-teaming` `CI/CD supply-chain security` `Static analysis` `Least-privilege tool policies` `OAuth flows` `Secrets hygiene`

**Languages**
`TypeScript` `Python` `SQL` `Java` `Kotlin`

**Backend & Web**
`Node.js` `FastAPI` `Next.js` `Django` `PostgreSQL` `REST APIs`

**Quality & Ops**
`Vitest` `Pytest` `GitHub Actions` `Docker` `Linux` `Git`

## Let's connect

I'm open to internships and collaborations in **applied AI engineering, LLM/agent security, and secure AI systems**.

- Email: [madeshandykrisnanda@gmail.com](mailto:madeshandykrisnanda@gmail.com)
- LinkedIn: [Made Shandy Krisnanda](https://www.linkedin.com/in/made-shandy-krisnanda-43ba86260)
