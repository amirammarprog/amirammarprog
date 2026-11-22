<!--
  Profile README for github.com/amirammarprog
  Edit freely: each section is independent. Widgets are plain image links,
  so a broken one can be deleted without touching the rest.
-->

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=190&section=header&text=Mohammed%20Amir%20Ammar&fontColor=ffffff&fontSize=42&fontAlignY=36&desc=Full-Stack%20Developer%20%C2%B7%20TypeScript%20%C2%B7%20React%20%C2%B7%20Node.js&descSize=17&descAlignY=58" alt="Mohammed Amir Ammar, Full-Stack Developer" width="100%" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/mohammedamir-ammar/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:mohammedamir.ammar@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Open%20to-Junior%20Full--Stack%20roles%20%C2%B7%20Remote-16a34a?style=for-the-badge" alt="Open to junior full-stack roles, remote" />
</p>

## Hi, I'm Amir 👋

I build full-stack web applications for real businesses. Over the past months I've built
the internal tools and websites of an industrial group in Tunisia (**SMCP Industrie / SMCP Metal**) and a few other local businesses:
a sales CRM, a stock and cutting-management platform, B2B websites, and a marketplace for metal and plastic offcuts.

I work across the whole stack: database schema, REST APIs, authentication and roles, React front ends,
PDF generation, multilingual UIs (French, Arabic RTL, English), tests, and deployment.

## 🛠️ Tech stack

These are the tools I use in my projects, not a list of things I've read about.

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

> 🔒 These projects belong to the companies I built them for, so the repositories are private.
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

Built for the SMCP Industrie sales team to manage prospects, clients, field visits, and the pipeline.

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
| **SMCP Metal website (v2)** | Company site pre-rendered in FR/AR/EN, quote requests with validated file uploads (PDF, DWG, DXF, STEP), anti-spam, and strict security headers | TypeScript, Express 5, Drizzle, React Router 7 |
| **SMCP platform (v1)** | Product catalogue, client onboarding, quote generation, stock arrivals, and an admin dashboard | Express 5, Prisma, PostgreSQL, React, jsPDF |
| **HARDMAT** | B2B website for engineering plastics (POM-C, PEEK, FR4) | Express, Prisma, PostgreSQL, React |
| **2SLC delivery slips** | Delivery slip app with yearly numbering, A4 PDF output, PostgreSQL sessions, CSRF protection, and Zod validation | Express, PostgreSQL, React, PDFKit |
| **Locatek** | Equipment rental management: rentals, payments, maintenance, and generated documents | Express, Prisma, SQLite, Docker |

## 🌱 Right now

- Building out **SMCP CRM**, the project I'm most active on. Its shared package is set up for future mobile and desktop clients.
- Learning **AI engineering**: LLM apps with OpenAI and LangChain, agents and memory with LangGraph, MCP, and vector search with Pinecone.
- Moving my projects to **TypeScript end to end**. The CRM, the marketplace, and the new SMCP website are typed front to back.

## 📜 Certificates

**AI Engineer** and **AI Agent Engineer** coursework on [365 Data Science](https://365datascience.com/), 17 courses completed in 2026. Click a title to open its certificate.

- **AI agents:** [Intro to AI Agents and Agentic AI](certificates/CC-FC068CEF92.pdf) · [AI Agent Architecture](certificates/CC-30EB5A693A.pdf) · [AI Agents in Practice](certificates/CC-B5574C126E.pdf) · [Evaluating AI Agents](certificates/CC-D55AEE0E96.pdf) · [MCPs for Everyone](certificates/CC-ADCE065DBE.pdf) · [Conversational AI Memory with LangGraph](certificates/CC-798808029D.pdf)
- **LLMs & NLP:** [Intro to LLMs](certificates/CC-45F7C18842.pdf) · [Intro to NLP for AI](certificates/CC-9D8CABD5FF.pdf) · [Chat Applications with OpenAI and LangChain](certificates/CC-C5080E7C16.pdf) · [LLM Engineering with Streamlit and OpenAI](certificates/CC-F47E3C2CF6.pdf) · [Vector Databases with Pinecone](certificates/CC-69D8071CD6.pdf)
- **Python, data & ML:** [Introduction to Python](certificates/CC-AFD3A770C1.pdf) · [Data Preprocessing with NumPy](certificates/CC-A2528C1637.pdf) · [Data Cleaning with pandas](certificates/CC-B3ED5B308F.pdf) · [Data Visualization (Python, R, Tableau, Excel)](certificates/CC-412E5771B6.pdf) · [Deep Learning with TensorFlow 2](certificates/CC-D25EE8E4A5.pdf)
- **Tools:** [Git and GitHub](certificates/CC-85233E11B1.pdf)

## 🎯 What I'm looking for

A **Junior Full-Stack Developer / Software Engineer** role, remote or abroad, on a team where I can ship
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

Recruiting for a junior full-stack role, or need someone to build an internal tool? I'd like to hear about it.

- **Email:** [mohammedamir.ammar@gmail.com](mailto:mohammedamir.ammar@gmail.com)
- **LinkedIn:** [linkedin.com/in/mohammedamir-ammar](https://www.linkedin.com/in/mohammedamir-ammar/)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=110&section=footer" alt="" width="100%" />
</p>
