
  # Hey, I'm Edward 👋

  Full-stack engineer building AI-powered applications with TypeScript, Node.js, Python, and React. Recent UCSB CS grad focused on production systems, novel architectures, and shipping
  quality code.

  **🎯 Currently seeking full-time engineering roles at startups** where I can build production systems, work with strong teams, and ship features that matter.

  ---

  ## ⚡ Highlights

  - 🏗️ Built **novel 3-layer DAG execution architecture** for AI query processing (2-5x parallel speedup)
  - 🧠 **Production-grade memory system** with 6-layer architecture, 5-stage entity resolution, and epistemic humility
  - 🧪 Custom **AI-powered E2E testing framework** validates non-deterministic LLM outputs
  - 🔐 Production systems with **OAuth 2.0, AES-256-GCM encryption, circuit breakers, RLS**
  - 📊 Evaluated **6 AI models across 125 safety scenarios** (97.6% pass rate with Claude 3)
  - 🚀 Shipped **live SaaS platform** with Stripe payments and multi-tenant architecture

  ---

  ## What I'm Building

  ### 🤖 [Tide (AI Email & Calendar Assistant)](https://github.com/ezhong0/tide)
  #### 🤖 [Version 0](https://github.com/ezhong0/aiassistant)
  Production-grade AI assistant that transforms natural language queries into complex multi-step operations across Google Workspace APIs.

  **Novel 3-Layer DAG Architecture:**
  - **Layer 1:** Query decomposition - Natural language → Structured execution graph
  - **Layer 2:** Parallel execution engine - 5 execution strategies (metadata filtering, semantic analysis, cross-reference, batch operations) with automatic dependency resolution
  achieving 2-5x speedup
  - **Layer 3:** Response synthesis - Structured results → Natural language with context-aware summarization

  **Technical Highlights:**
  - 72,000+ lines of production TypeScript/React with 80%+ test coverage
  - Stateless backend enables horizontal scaling with OAuth 2.0, AES-256-GCM token encryption, circuit breakers, rate limiting
  - Custom E2E testing framework validates non-deterministic LLM outputs using AI-powered judges (GPT-4, Claude) against ground truth datasets
  - React Native mobile app with offline-first architecture, AsyncStorage persistence, comprehensive onboarding flow
  - 700+ documented use cases covering inbox triage, commitment tracking, context recovery

  **Stack:** Node.js, TypeScript, PostgreSQL, OpenAI GPT-4, Anthropic Claude, React Native, Supabase, Docker

  ---

  ### 🧠 [Ontology-Aware Memory System](https://github.com/ezhong0/ontology-memory-llm)
  > Production-ready memory system that transforms LLM agents from stateless responders into experienced colleagues with perfect recall, business context awareness, and epistemic humility.
   11,864 lines of production Python with pure hexagonal architecture.

  <details>
  <summary><strong>🏗️ Architecture Highlights</strong></summary>

  **6-Layer Memory Architecture:**
  - **Layer 1:** Raw events (immutable audit trail, provenance tracking)
  - **Layer 2:** Entity resolution (5-stage hybrid: exact → alias → fuzzy → LLM coreference → domain lookup)
  - **Layer 3:** Episodic memory (events with semantic meaning, entity tracking)
  - **Layer 4:** Semantic memory (Subject-Predicate-Object triples with confidence decay)
  - **Layer 5:** Procedural memory (learned behavioral patterns)
  - **Layer 6:** Memory summaries (cross-session consolidation)

  **5-Stage Entity Resolution (95% Deterministic, 5% LLM):**
  - Stage 1: Exact match (70% of cases, <5ms)
  - Stage 2: User aliases (15% of cases, learned from prior interactions)
  - Stage 3: Fuzzy match using PostgreSQL pg_trgm (10% of cases, handles typos)
  - Stage 4: LLM coreference resolution (5% of cases, pronouns/demonstratives only)
  - Stage 5: Domain database lookup with lazy entity creation

  **Dual Truth Architecture:**
  - **Correspondence Truth:** Authoritative data from domain database (ERP systems)
  - **Contextual Truth:** Interpretive understanding from memory layers
  - Explicit conflict detection (memory vs. memory, memory vs. DB, temporal inconsistency)

  **Multi-Signal Retrieval:**
  - 5 weighted signals: semantic similarity (40%), entity overlap (25%), recency (20%), temporal coherence (10%), importance (5%)
  - pgvector for sub-50ms vector similarity search
  - Confidence decay with exponential formula (reaches 0.5 after 60 days without validation)

  **Epistemic Humility:**
  - System NEVER claims 100% certainty (MAX_CONFIDENCE = 0.95)
  - All semantic memories have confidence scores with decay
  - Conflicts are surfaced explicitly, never silently resolved

  **Technical Quality:**
  - Pure hexagonal architecture (domain layer has ZERO infrastructure imports)
  - 100% type coverage (mypy --strict mode)
  - 130+ tests with 85% coverage (70% unit, 20% integration, 10% E2E)
  - Property-based testing with Hypothesis for invariant validation
  - Structured logging (JSON) for production observability

  **Stack:** Python 3.11+, FastAPI, PostgreSQL 15, pgvector, SQLAlchemy 2.0 (async), OpenAI, Anthropic Claude, Alembic, pytest, mypy, Ruff

  **Performance:** <200ms for deterministic paths, <800ms with LLM extraction, ~$0.002 per conversational turn

  </details>

  ---

  ### 🛡️ [AI Safety Evaluation Benchmark](https://github.com/ezhong0/humanebench)
  > Production benchmark evaluating AI chatbot safety across 8 critical domains (mental health, medical emergencies, financial scams, abuse). Tested 6 AI models across 125 scenarios—Claude
   3 Haiku achieved 97.6% safety pass rate.

  <details>
  <summary><strong>📊 Framework Details</strong></summary>

  **Evaluation Framework:**
  - Tests AI systems across 8 critical safety domains: mental health crises, medical emergencies, financial scams, relationship abuse, privacy violations, social isolation, self-harm, and
  misinformation
  - Multi-dimensional scoring rubric: Safety & Dignity (40%), Long-term Wellbeing (40%), Transparency (20%)
  - 125 unique test scenarios across 4 harm pattern types and 3 vulnerability levels

  **Research Results:**
  - Evaluated 6 leading AI models (Claude 3, GPT-4, Gemini, Grok, Llama)
  - Claude 3 Haiku achieved highest score: 4.90/5.0 with 97.6% safety pass rate
  - Comprehensive HTML reporting with Chart.js visualizations and failure analysis

  **Stack:** Python 3.10+, AISI Inspect, OpenAI, Anthropic, Google Gemini, Pydantic, Jinja2

  </details>

  ---

  ### 💼 [Invoice Automation SaaS](https://csvtoinvoice.vercel.app)
  > Live SaaS platform automating PDF invoice generation from spreadsheets. Handles bulk processing (10K rows in 1.5s, 100 invoices in 5s) with Stripe payments and multi-tenant
  architecture.

  <details>
  <summary><strong>🔧 Technical Details</strong></summary>

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

  </details>

  ---

  ## Tech Stack

  **Languages:** TypeScript, Python, JavaScript, SQL
  **Backend:** Node.js, Express, Flask, FastAPI, PostgreSQL
  **Frontend:** React, React Native, Next.js
  **AI/ML:** OpenAI, Anthropic, LLM Integration, Prompt Engineering, Vector Search
  **DevOps:** Docker, GitHub Actions, Railway, Vercel
  **Architecture:** Hexagonal/Clean Architecture, Domain-Driven Design, Event Sourcing

  ---

  ## Let's Connect

  - 📧 **Email:** [edwardrzhong@gmail.com](mailto:edwardrzhong@gmail.com)
  - 💼 **LinkedIn:** [linkedin.com/in/edwardzhong0](https://linkedin.com/in/edwardzhong0)
  - 🔗 **Portfolio:** Check out pinned repos below

  ---

  <sub>Building in public. Learning in public. Shipping quality code.</sub>
