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

## Featured: Agent Warden

**[Agent Warden](https://github.com/azzelll/agent-warden)**: a red-team harness and a four-layer firewall against indirect prompt injection in tool-using LLM agents.

- **104 attacks**: 5 attacker goals × 3 injection vectors × 8 techniques (English and Indonesian, base64, fake system tags, forged conversation turns, impersonation).
- **4 independent defense layers**: spotlighting, an injection scanner, a tool-call policy whose capabilities come only from the user's prompt (with taint tracking), and an output filter.
- **Deterministic scoring** from observable side effects, never an LLM judge, reported with 95% confidence intervals.
- Against a worst-case agent that obeys every injected instruction: **99% → 0% attack success, with 100% of benign tasks still working.** No single layer was enough on its own.
- Ships as an **MCP gateway** (`warden-gateway`) that puts the same policy in front of any stdio MCP server. A workshop paper draft is in progress.

## Selected projects

| Project | What I built | Core stack |
| --- | --- | --- |
| [Agent Warden](https://github.com/azzelll/agent-warden) | Prompt-injection red-team harness, tool-call firewall and MCP gateway for LLM agents. | TypeScript, Ollama, MCP, Vitest |
| [AIKO: Academic Inbox & Knowledge Organizer](https://github.com/azzelll/academic-inbox-knowledge-organizer) | Discord bot for a class server: each student binds their own SCELE feed for private deadline lists and a daily DM, asks course-material questions answered with page-level citations (hybrid BM25 + embedding retrieval), and the owner gets Gmail watch rules judged by a local LLM plus GitHub worklog drafts. | TypeScript, discord.js, Ollama, RAG, PostgreSQL, Docker |
| [SRASTA WiFi CSI](https://github.com/azzelll/SRASTA-WiFi-CSI) | WiFi-CSI activity and fall-detection pipeline: TCN-Lite training, INT8 TFLite inference on Raspberry Pi, and Blynk IoT alerts. **GEMASTIK finalist (IoT).** | Python, TensorFlow Lite, Raspberry Pi, ESP32 |
| [Carda](https://github.com/azzelll/Carda) | Privacy-first Android prototype for on-device fingertip PPG wellness measurements, designed with explicit safety constraints. **GEMASTIK finalist (Software Development).** | Kotlin, Jetpack Compose, CameraX, TFLite |
| [Environmental AI / Ecometric](https://github.com/azzelll/environmental-ai-project) | Multimodal environmental-quality system for air, water and soil prediction. The broader Ecometric product won **2nd place** at the Pekan RISTEK Mini Hackathon 2025. | FastAPI, Python, ML, Next.js, Firebase |

## Highlights

- 🏆 **GEMASTIK Finalist, Internet of Things division:** [SRASTA](https://github.com/azzelll/SRASTA-WiFi-CSI), contactless activity and fall detection from WiFi CSI running on a Raspberry Pi.
- 🏆 **GEMASTIK Finalist, Software Development division:** [Carda](https://github.com/azzelll/Carda), a privacy-first on-device PPG wellness app for Android.
- 🥈 **2nd Place, Pekan RISTEK Mini Hackathon 2025:** shipped Ecometric as a working full-stack MVP in under 48 hours.
- 🥈 **2nd Place, Pekan RISTEK Data Competition 2025:** LightGBM/XGBoost earthquake early-detection system with cross-validation and out-of-fold blending.
- 🏅 **HFLP Awardee 2026.**

## Tech toolbox

**AI & ML**
`LLM agents` `Tool calling` `RAG` `Ollama` `MCP` `scikit-learn` `LightGBM` `XGBoost` `TensorFlow` `TFLite` `MLflow`

**Security**
`Threat modeling` `Prompt-injection red-teaming` `Least-privilege tool policies` `OAuth flows` `Secrets hygiene`

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
