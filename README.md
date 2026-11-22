<!--
  Profile README for github.com/amirammarprog
  Edit freely: each section is independent. Widgets are plain image links,
  so a broken one can be deleted without touching the rest.
-->

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=190&section=header&text=Mohammed%20Amir%20Ammar&fontColor=ffffff&fontSize=42&fontAlignY=36&desc=AI%20Engineer%20%2F%20Software%20Engineer%20%C2%B7%20TypeScript%20%C2%B7%20React%20%C2%B7%20Node.js&descSize=17&descAlignY=58" alt="Mohammed Amir Ammar, AI Engineer / Software Engineer" width="100%" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/mohammedamir-ammar/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:mohammedamir.ammar@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Open%20to-AI%20%26%20Software%20Engineering%20roles%20%C2%B7%20Remote-16a34a?style=for-the-badge" alt="Open to AI and software engineering roles, remote" />
</p>

## Hi, I'm Amir 👋

I build full-stack web applications for real businesses. Over the past months I've built
the internal tools and websites of an industrial group in Tunisia (**SMCP**) and a few other local businesses:
a sales CRM, a stock and cutting-management platform, B2B websites, and a marketplace for metal and plastic offcuts.

I work across the whole stack: database schema, REST APIs, authentication and roles, React front ends,
PDF generation, multilingual UIs (French, Arabic RTL, English), tests, and deployment.

## 🛠️ Tech stack

The AI group comes from my [certified coursework](#-certifications) and my open-source projects [Multilingual AI Support Agent](https://github.com/amirammarprog/multilingual-ai-support-agent) and [Quote Copilot](https://github.com/amirammarprog/quote-copilot). Everything after it is what I use in my professional projects.

**AI engineering & machine learning**

<p>
  <img src="https://skillicons.dev/icons?i=python,tensorflow,r&theme=dark" alt="Python, TensorFlow, R" />
</p>

- **LLMs & agents:** OpenAI API · LangChain · LangGraph (agents with conversational memory) · MCP (Model Context Protocol) · agent architecture and evaluation
- **Retrieval & NLP:** pgvector hybrid search (vector + full-text) · cross-encoder reranking · Pinecone · multilingual NLP (Arabic, French, English) · Streamlit for LLM app front ends
- **Python back end:** FastAPI · SQLAlchemy · Alembic · Pydantic · pytest
- **Data & ML:** pandas · NumPy · machine learning in Python · deep learning with TensorFlow 2 · data visualization (Python, R, Tableau, Excel)

**Languages & front end**

<p>
  <img src="https://skillicons.dev/icons?i=ts,js,html,css,react,vite,tailwind&theme=dark" alt="TypeScript, JavaScript, HTML, CSS, React, Vite, Tailwind CSS" />
</p>

React 19 · React Router 7 (SSR and pre-rendering) · Tailwind CSS 4 · TanStack Query · i18next · Recharts · Motion

**Back end & data**

<p>
  <img src="https://skillicons.dev/icons?i=nodejs,express,nestjs,prisma,postgres,sqlite&theme=dark" alt="Node.js, Express, NestJS, Prisma, PostgreSQL, SQLite" />
</p>

Express 5 · NestJS 11 · Prisma · Drizzle ORM · PostgreSQL (Neon, PGlite) · Socket.IO · Zod · JWT and session auth · Argon2 / bcrypt · PDFKit / pdf-lib · Nodemailer

**Testing, tooling & deployment**

<p>
  <img src="https://skillicons.dev/icons?i=vitest,docker,githubactions,git,pnpm&theme=dark" alt="Vitest, Docker, GitHub Actions, Git, pnpm" />
</p>

Vitest · Playwright + axe (accessibility) · Biome · Docker · GitHub Actions CI/CD · Render

## 🚀 Featured work

### [Multilingual AI Support Agent](https://github.com/amirammarprog/multilingual-ai-support-agent): customer support in Arabic, Tunisian Arabic, French and English

<a href="https://github.com/amirammarprog/multilingual-ai-support-agent"><img src="https://img.shields.io/badge/repo-public-2563eb?style=flat-square&logo=github" alt="Public repository" /></a>
<a href="https://github.com/amirammarprog/multilingual-ai-support-agent/actions/workflows/ci.yml"><img src="https://github.com/amirammarprog/multilingual-ai-support-agent/actions/workflows/ci.yml/badge.svg" alt="CI status" /></a>
<a href="https://github.com/amirammarprog/multilingual-ai-support-agent/actions/workflows/evals.yml"><img src="https://github.com/amirammarprog/multilingual-ai-support-agent/actions/workflows/evals.yml/badge.svg" alt="Evaluation status" /></a>

A 24/7 support agent for e-commerce shops, by text or voice. It answers only from the shop's documents and live data, and when it doesn't know, it says so and offers a human.

- LangGraph agent: guardrails → cheap/capable model router → planner → permission-checked tools → answer from evidence → validation (numbers not found in the evidence are rejected)
- Hybrid RAG on PostgreSQL + pgvector: full-text and vector search, multilingual reranking, cross-lingual queries, citations
- 7 tools (orders, stock, products, tickets, hand-off) served over MCP, with authorization in the backend and row-level security per shop
- Adversarial security tests (prompt injection, other customers' data, price manipulation, poisoned documents) and a 130-question evaluation in 4 languages in GitHub Actions
- React admin console and a 17 KB embeddable widget with Arabic right-to-left support

`Python` `FastAPI` `LangGraph` `PostgreSQL` `pgvector` `MCP` `React` `TypeScript` `Docker` `GitHub Actions` `Langfuse`

### [Quote Copilot](https://github.com/amirammarprog/quote-copilot): AI agent for industrial quote requests

<a href="https://github.com/amirammarprog/quote-copilot"><img src="https://img.shields.io/badge/repo-public-2563eb?style=flat-square&logo=github" alt="Public repository" /></a>
<a href="https://github.com/amirammarprog/quote-copilot/actions/workflows/ci.yml"><img src="https://github.com/amirammarprog/quote-copilot/actions/workflows/ci.yml/badge.svg" alt="CI status" /></a>
<img src="https://img.shields.io/badge/status-in%20progress-f59e0b?style=flat-square" alt="In progress" />

An AI agent that turns a customer's quote request email into a priced draft quote, which a person reviews and approves before anything is sent.

- LangGraph workflow: extract → retrieve → tool calls → price → draft → **human approval** → send, with customer memory ("same as last time but 20 mm thick")
- OpenAI structured outputs (Pydantic) read the request. The model never computes prices: they come from a tested pricing tool
- MCP server exposing 4 tools (`search_stock`, `get_material`, `price_cut`, `create_quote`) over a seeded Postgres database
- Retrieval of material datasheets and past quotes with Pinecone
- Eval harness in GitHub Actions: field accuracy, price error, tool-call correctness, cost and latency per request
- Streamlit reviewer UI: inbox, extracted fields, quote preview, approve, edit or reject

`Python` `LangGraph` `OpenAI API` `MCP` `Pinecone` `PostgreSQL` `Streamlit` `Docker` `GitHub Actions`

> 🔒 The projects below belong to the companies I built them for, so the repositories are private.
> I'm happy to walk you through the code and architecture on a call.

### LiquiStock: marketplace for metal and plastic offcuts

An online shop where machinable offcuts are sold piece by piece, with a full back office behind it.

- Server-rendered catalogue with per-shape pages, a command palette (⌘K), and FR/EN routing
- Accounts with Argon2 sessions, a guest cart merged at login, and checkout that reserves stock for 15 minutes
- Back office: stock CRUD, bulk pricing, CSV import/export, Code128 labels, order workflow, content editors
- Quality gates in CI: Biome, type checking, Vitest, i18n key parity, WCAG contrast checks, and Playwright + axe e2e across 2 languages × 2 themes
- Docker images built in GitHub Actions and pushed to GHCR, then deployed to staging and production on Render

`TypeScript` `React Router 7` `Drizzle` `PostgreSQL` `Tailwind 4` `Vitest` `Playwright` `Docker` `GitHub Actions`

### SMCP CRM: sales CRM for an industrial distributor

Built for the SMCP sales team to manage prospects, clients, field visits, and the pipeline.

- Monorepo: NestJS API, React web app, and a shared package for business rules and design tokens
- Role-based access: no self-sign-up, only managers create accounts, and rules enforced server-side (for example, at least one active manager)
- Real-time updates with Socket.IO, Excel and PDF exports, and file uploads
- French, Arabic (right-to-left), and English, plus light and dark themes saved per user

`TypeScript` `NestJS 11` `Prisma` `PostgreSQL 17` `React 19` `Socket.IO` `Docker`

### SMCP Express: internal cutting and stock-management platform

Internal B2B platform for cutting and selling plastic and metal stock across two sites.

- Three roles (admin, technician, operator) with a per-module permission matrix
- Orders, custom-cut pricing by weight and density, quotes, cash register, exit slips, and import tracking
- Idempotent seeding that never overwrites live stock, plus scripted acceptance checks for each release

`JavaScript` `Express` `Prisma` `PostgreSQL` `React` `TanStack Query` `Socket.IO`

### Also built

| Project | What it is | Stack |
| --- | --- | --- |
| **SMCP website (v2)** | Company site pre-rendered in FR/AR/EN, quote requests with validated file uploads (PDF, DWG, DXF, STEP), anti-spam, and strict security headers | TypeScript, Express 5, Drizzle, React Router 7 |
| **SMCP platform (v1)** | Product catalogue, client onboarding, quote generation, stock arrivals, and an admin dashboard | Express 5, Prisma, PostgreSQL, React, jsPDF |
| **HARDMAT** | B2B website for engineering plastics (POM-C, PEEK, FR4) | Express, Prisma, PostgreSQL, React |
| **2SLC delivery slips** | Delivery slip app with yearly numbering, A4 PDF output, PostgreSQL sessions, CSRF protection, and Zod validation | Express, PostgreSQL, React, PDFKit |
| **Locatek** | Equipment rental management: rentals, payments, maintenance, and generated documents | Express, Prisma, SQLite, Docker |

## 🌱 Right now

- Building out **SMCP CRM**, the project I'm most active on. Its shared package is set up for future mobile and desktop clients.
- Next for the **[Multilingual AI Support Agent](https://github.com/amirammarprog/multilingual-ai-support-agent)**: running its full evaluation with an LLM (only offline results are published so far) and recording a demo.
- Building **[Quote Copilot](https://github.com/amirammarprog/quote-copilot)**. Next steps: LLM evals in CI on a larger test set, and a recorded demo.
- Moving my projects to **TypeScript end to end**. The CRM, the marketplace, and the new SMCP website are typed front to back.

## 📜 Certifications

- **Certified Cybersecurity Educator Professional (CCEP)**: Red Team Leaders, exam passed October 2026 · [verify](https://courses.redteamleaders.com/exam-completion/40fe651e3639fb41)
- **AWS Certified Generative AI Developer – Professional (AIP-C01), official practice question set**: AWS Training & Certification, completed October 2026 · [certificate](certificates/AWS-AIP-C01-practice-question-set.pdf)

**AI Engineer** and **AI Agent Engineer** coursework on [365 Data Science](https://365datascience.com/): 19 courses completed in 2026. Each title links to its verification page.

- **AI agents:** [Intro to AI Agents and Agentic AI](https://learn.365datascience.com/c/558fb78b5e/) · [AI Agent Architecture](https://learn.365datascience.com/c/704e98c783/) · [AI Agents in Practice](https://learn.365datascience.com/c/98a75a6517/) · [Evaluating AI Agents](https://learn.365datascience.com/c/afbf8381f9/) · [MCPs for Everyone](https://learn.365datascience.com/c/d9457657d9/) · [Conversational AI Memory with LangGraph](https://learn.365datascience.com/c/fc84847fa6/)
- **AI, LLMs & NLP:** [Intro to AI](https://learn.365datascience.com/c/1c00d6359b/) · [Intro to LLMs](https://learn.365datascience.com/c/77b4a0cb1e/) · [Intro to NLP for AI](https://learn.365datascience.com/c/235b3b93f2/) · [Chat Applications with OpenAI and LangChain](certificates/CC-C5080E7C16.pdf) · [LLM Engineering with Streamlit and OpenAI](https://learn.365datascience.com/c/c13b28ba1f/) · [Vector Databases with Pinecone](https://learn.365datascience.com/c/03eecf4243/)
- **Python, data & ML:** [Introduction to Python](https://learn.365datascience.com/c/3734ecc93c/) · [Data Preprocessing with NumPy](https://learn.365datascience.com/c/aca3a6db82/) · [Data Cleaning with pandas](https://learn.365datascience.com/c/e40c19d396/) · [Data Visualization (Python, R, Tableau, Excel)](https://learn.365datascience.com/c/00a97dc7e2/) · [Machine Learning in Python](https://learn.365datascience.com/c/61c5c2f5c2/) · [Deep Learning with TensorFlow 2](https://learn.365datascience.com/c/54573c6d3c/)
- **Tools:** [Git and GitHub](https://learn.365datascience.com/c/1a842cdcbc/)

## 🎯 What I'm looking for

A **junior AI Engineer or Software Engineer** role, remote or abroad, on a team where I can ship
real features, get code reviews, and grow. Most of what I've built so far turns a company's day-to-day process
(sales, stock, quotes, delivery slips) into a web app.

<!--
  Activity graph: hidden for now because GitHub only counts public contributions
  until "Include private contributions on my profile" is turned on.
  After turning that setting on, delete this comment's opening and closing lines to show it.

## 📈 Activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=amirammarprog&bg_color=0d1117&color=c9d1d9&line=3b82f6&point=93c5fd&area=true&area_color=1d4ed8&hide_border=true&custom_title=Contribution%20activity" />
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=amirammarprog&bg_color=ffffff&color=1f2328&line=2563eb&point=1d4ed8&area=true&area_color=bfdbfe&hide_border=true&custom_title=Contribution%20activity" alt="Contribution activity graph" width="100%" />
  </picture>
</p>
-->

## 📫 Let's talk

Recruiting for a junior AI or software engineering role, or need someone to build an internal tool? I'd like to hear about it.

- **Email:** [mohammedamir.ammar@gmail.com](mailto:mohammedamir.ammar@gmail.com)
- **LinkedIn:** [linkedin.com/in/mohammedamir-ammar](https://www.linkedin.com/in/mohammedamir-ammar/)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=110&section=footer" alt="" width="100%" />
</p>
