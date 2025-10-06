# Hey, I'm Edward 👋

Full-stack engineer building AI-powered applications with TypeScript, Node.js, and React. Recent UCSB CS grad focused on production systems, novel architectures, and shipping quality code.

## What I'm Building

### 🤖 [AI Email & Calendar Assistant](https://github.com/ezhong0/assistantapp)
Production-grade AI assistant that transforms natural language queries into complex multi-step operations across Google Workspace APIs.

**Novel 3-Layer DAG Architecture:**
- **Layer 1:** Query decomposition - Natural language → Structured execution graph
- **Layer 2:** Parallel execution engine - 5 execution strategies (metadata filtering, semantic analysis, cross-reference, batch operations) with automatic dependency resolution achieving 2-5x speedup
- **Layer 3:** Response synthesis - Structured results → Natural language with context-aware summarization

**Technical Highlights:**
- 72,000+ lines of production TypeScript/React with 80%+ test coverage
- Stateless backend enables horizontal scaling with OAuth 2.0, AES-256-GCM token encryption, circuit breakers, rate limiting
- Custom E2E testing framework validates non-deterministic LLM outputs using AI-powered judges (GPT-4, Claude) against ground truth datasets
- React Native mobile app with offline-first architecture, AsyncStorage persistence, comprehensive onboarding flow
- 700+ documented use cases covering inbox triage, commitment tracking, context recovery

**Stack:** Node.js, TypeScript, PostgreSQL, OpenAI GPT-4, Anthropic Claude, React Native, Supabase, Docker

---

### 🛡️ [AI Safety Evaluation Benchmark](https://github.com/ezhong0/humanebench)
Production benchmark for evaluating AI chatbot safety and alignment across vulnerable user scenarios.

**Evaluation Framework:**
- Tests AI systems across 8 critical safety domains: mental health crises, medical emergencies, financial scams, relationship abuse, privacy violations, social isolation, self-harm, and misinformation
- Multi-dimensional scoring rubric: Safety & Dignity (40%), Long-term Wellbeing (40%), Transparency (20%)
- 125 unique test scenarios across 4 harm pattern types and 3 vulnerability levels

**Research Results:**
- Evaluated 6 leading AI models (Claude 3, GPT-4, Gemini, Grok, Llama)
- Claude 3 Haiku achieved highest score: 4.90/5.0 with 97.6% safety pass rate
- Comprehensive HTML reporting with Chart.js visualizations and failure analysis

**Stack:** Python 3.10+, AISI Inspect, OpenAI, Anthropic, Google Gemini, Pydantic, Jinja2

---

### 💼 [Invoice Automation SaaS](https://csvtoinvoice.vercel.app)
Live full-stack SaaS platform that automates PDF invoice generation from spreadsheet data.

**Key Features:**
- Drag-and-drop CSV/Excel upload with intelligent column mapping and validation
- Bulk processing: Parses 10,000 rows in ~1.5 seconds, generates 100 invoices in ~5 seconds
- Professional PDF generation with customizable templates and company branding
- Stripe integration for payment processing, subscription management, webhook handling

**Architecture:**
- Next.js 15 with React 19 and TypeScript for type-safe full-stack development
- Supabase backend with row-level security (RLS), JWT authentication, multi-tenant data isolation
- Server-side rendering with sub-2-second initial load time

**Stack:** Next.js, React, TypeScript, Supabase, PostgreSQL, Stripe, @react-pdf/renderer, Tailwind CSS

## Tech Stack

**Languages:** TypeScript, Python, JavaScript, SQL
**Backend:** Node.js, Express, Flask, PostgreSQL
**Frontend:** React, React Native, Next.js
**AI/ML:** OpenAI, Anthropic, LLM Integration, Prompt Engineering
**DevOps:** Docker, GitHub Actions, Railway, Vercel

## What I'm Looking For

Currently seeking full-time engineering roles at startups where I can:
- Build production systems that scale
- Work with strong engineering teams
- Ship features that matter to real users

## Let's Connect

- 📧 **Email:** [edwardrzhong@gmail.com](mailto:edwardrzhong@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/edwardzhong0](https://linkedin.com/in/edwardzhong0)
- 🔗 **Portfolio:** Check out pinned repos below

---

<sub>Building in public. Learning in public. Shipping quality code.</sub>
