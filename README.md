<div align="center">

# Phaneendra Gavara

**AI/ML Engineer · Data Scientist · I build AI systems that actually reach production**

[![Portfolio](https://img.shields.io/badge/Portfolio-phaneendragavara.dev-8b5cf6?style=for-the-badge&logo=vercel&logoColor=white)](https://phaneendragavara.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/phaneendra-gavara)
[![Email](https://img.shields.io/badge/Email-Reach%20out-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](https://phaneendragavara.dev/contact)
[![Open to Work](https://img.shields.io/badge/Open%20to-AI%2FML%20Roles-34d399?style=for-the-badge)](https://phaneendragavara.dev/contact)

</div>

---

## Currently

🔬 &nbsp;**Visiting Researcher** — ASU School of Computing and Augmented Intelligence *(Aug 2026 – Present)*
&nbsp;&nbsp;&nbsp;&nbsp;AI-driven approaches for blockchain: ML model analysis, and improving blockchain security, scalability and efficiency.

🎓 &nbsp;**M.S. Data Science**, Arizona State University — GPA 3.90/4.0 *(graduated May 2026)*

🚀 &nbsp;Building **AgentForge** — a production platform for deploying, evaluating and governing autonomous AI agents

💼 &nbsp;Open to **AI/LLM Engineer**, **ML Engineer** and **Data Scientist** roles · authorised to work in the US without sponsorship

```python
class Phaneendra:
    role       = ["AI/LLM Engineer", "ML Engineer", "Data Scientist"]
    focus      = ["Agentic AI", "RAG Systems", "LLM Evaluation", "MLOps"]
    building   = "AgentForge — deploy, evaluate and govern AI agents"
    philosophy = "A model in a notebook is a hypothesis. Shipped, it's a product."
```

---

## Featured Projects

### 🤖 AgentForge — Agent-Native Platform
> *"Vercel for AI agents."* Define an agent, give it tools, safety rules and a budget, push it live, and watch it run with guardrails already in place.

Most AI tooling logs a single model call. AgentForge is built for **agents** — multi-step reasoning, real tool calls, decisions that need a leash.

- **Agent runtime** — think → act → observe loop with tool orchestration
- **Safety enforcement** — PII + policy checks at two checkpoints (block / warn / log) and an LLM scope-guard that confines an agent to its topic
- **Budget caps** — hard per-agent daily spend limits enforced *before* a run starts
- **Evaluation** — LLM-as-judge scoring with version-to-version comparison (pass rate, latency, cost)
- **Observability** — OpenTelemetry traces in Grafana, per-step tokens and cost
- **BYOK, multi-provider** — bring your own encrypted key for 100+ providers via LiteLLM
- **Taken fully to production on AWS/EKS** — Terraform IaC, Helm, gated GitHub Actions pipeline, HTTPS + WAF — then a clean teardown to **$0**, proving the whole lifecycle rather than just the demo

`Solo build · ~4 weeks · ~16,800 LOC · 160+ tests · 5 microservices + Go CLI + Python SDK`

**Tech:** Python · FastAPI · Go · React · TypeScript · LiteLLM · PostgreSQL · Redis · OpenTelemetry · Grafana · Docker · Terraform · Helm · AWS (EKS, RDS, ElastiCache, ALB, WAF)

🔗 [GitHub](https://github.com/PHANI465/AGENTFORGE)

---

### 📊 InsightHub — AI-Powered Business Analytics Platform
Full-stack Azure analytics platform ingesting 230,000+ rows through a star-schema ETL pipeline, serving insights via FastAPI, a React dashboard and a GPT-4o RAG search engine. Deployed and live.

- Python ETL: 7 CSVs → star schema (6 dims, 3 facts) in Azure SQL, 230,000+ rows
- Columnstore index cut FactSales aggregation from **~8s to under 1s** on 119,652 rows
- Hybrid RAG: BM25 + ada-002 embeddings + Azure AI Search semantic re-ranking
- FastAPI with JWT auth + RBAC (Admin / Analyst / Viewer), 14 endpoints
- Bicep IaC for all 13 Azure resources with Key Vault references — zero plaintext credentials

**Tech:** Python · FastAPI · Azure SQL · Azure OpenAI · Azure AI Search · React 18 · TypeScript · Bicep IaC

🔗 [GitHub](https://github.com/PHANI465/insighthub) · [Live Demo](https://insighthub-five.vercel.app)

---

### 🧪 ASU LLM Evaluation Pipeline
Automated CI/CD pipeline that scores a university RAG chatbot on every push, making LLM quality enforceable like unit tests.

- **6 quality gates block deployment** — faithfulness ≥ 0.80, hallucination ≤ 10%, relevancy ≥ 0.75
- GPT-4o-mini as judge: **25× cheaper** (~$0.87/run vs ~$21.75) with no measured quality drop
- Live React dashboard with trend charts across 50 runs and a per-question breakdown

`Latest run: 6/6 gates PASS · Faithfulness 1.00 · Hallucination 0% · $0.087`

**Tech:** Python · LangChain · RAGAS · GPT-4o · Pinecone · GitHub Actions · React

🔗 [GitHub](https://github.com/PHANI465/asu-llm-eval)

---

### More Work

| Project | What it does | Tech |
|---|---|---|
| 🏭 **[Industrial AI Copilot](https://github.com/PHANI465/Tracker-Hacker)** | Sub-second anomaly detection across 4 live sensor streams, with a full incident pipeline: audio alert → work order → technician email | Next.js · TypeScript · Python · Resend |
| 🗺️ **[TravelIQ](https://github.com/PHANI465/TravelIQ)** | Feasibility-checked travel itinerary in under 90s: OR-Tools VRPTW routing, SARIMAX crowd forecasting, DistilBERT review sentiment | Python · OR-Tools · SARIMAX · DistilBERT · GPT-4o |
| 🫘 **[Republic of Bean](https://github.com/PHANI465/Republic-of-Bean)** | Multi-agent conversational system on LangGraph, with an MCP layer exposing PostgreSQL-backed APIs to the LLM as callable tools | LangGraph · Claude API · FastAPI · PostgreSQL · MCP |
| 👁️ **[Crowd Anomaly Detection](https://github.com/PHANI465/CrowdAnomalyDetection)** | CNN that learns normal crowd behaviour from video and flags anomalies with frame-level heatmaps | PyTorch · OpenCV · CNNs |
| ☎️ **AI Voice Turing Test** 🥉 | Distinguishes human from AI-generated calls via MFCC features + transcript sentiment. **3rd place, ASU Social Bias Hackathon** | Transformers · Librosa · HuggingFace |
| 🌐 **[This Portfolio](https://phaneendragavara.dev)** | 3 live-switching themes, an AI assistant on GPT-4o mini + Pinecone RAG, and an interactive terminal | Next.js 14 · TypeScript · Tailwind · Pinecone |

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**AI / ML**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![RAGAS](https://img.shields.io/badge/RAGAS-8b5cf6?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-D97757?style=flat-square)

**Backend & Data**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-5AD6E6?style=flat-square&logo=pinecone&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

---

## Certifications

<p align="center">
<a href="https://www.credly.com/badges/f8d45105-4913-4ebb-9353-36635ff76f65/public_url"><img src="https://img.shields.io/badge/AWS-Solutions%20Architect%20Associate-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS Certified Solutions Architect - Associate"></a>
<a href="https://www.credly.com/badges/c4f2a25d-6ba4-4349-a5e2-de8bf03459f3"><img src="https://img.shields.io/badge/AWS-AI%20Practitioner-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS Certified AI Practitioner"></a>
<img src="https://img.shields.io/badge/Anthropic-4%20Certificates-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Anthropic certificates">
</p>

- **AWS Certified Solutions Architect – Associate** · [Verify](https://www.credly.com/badges/f8d45105-4913-4ebb-9353-36635ff76f65/public_url)
- **AWS Certified AI Practitioner** · [Verify](https://www.credly.com/badges/c4f2a25d-6ba4-4349-a5e2-de8bf03459f3)
- AI Fluency Framework & Foundations · Anthropic
- Introduction to Claude Cowork · Claude Code 101 · Claude 101 · Anthropic

---

## GitHub

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=PHANI465&theme=github_dark" alt="GitHub contribution summary for PHANI465" width="100%">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=PHANI465&theme=github_dark" alt="Top languages by repository" height="170">
<img src="https://streak-stats.demolab.com/?user=PHANI465&theme=github-dark-blue&hide_border=true" alt="GitHub contribution streak" height="170">

</div>

---

## What I'm Into

`LLM evaluation & quality gates for AI` · `Agentic systems and autonomous workflows` · `Bayesian statistics & probabilistic modelling` · `MLOps and production ML infrastructure` · `Human-centred, explainable AI`

---

<div align="center">

**[Portfolio](https://phaneendragavara.dev)** &nbsp;·&nbsp; **[LinkedIn](https://linkedin.com/in/phaneendra-gavara)** &nbsp;·&nbsp; **[GitHub](https://github.com/PHANI465)**

*Building AI that is useful, explainable and human-centred.*

</div>
