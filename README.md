# Hi, I'm Tanmay Sharma

MS in Computing (AI) from the University of Utah. Based in Bangalore.

I tend to think across a lot of layers at once. That's why alongside my AI degree I studied entrepreneurial finance, patent law, and human-computer interaction. Not because I had to but because I was curious about how technology actually lands in the real world across business, legal, and human layers.

I'm more energized by figuring out what needs to be built and why than by implementing what's already been decided.

---

## What I'm Working On

**SEC Regulatory Document Interpreter**

    A pipeline that takes raw SEC regulatory PDFs and produces structured obligations with CFR citations, then
    interprets each one with grounding in the SEC's own reasoning. The core insight: extraction is not the hard part —
    interpretation is. Figuring out what an obligation means operationally, what is ambiguous, and what a company
    actually needs to change is where the real difficulty lives.

    Built and tested on the 2023 SEC Cybersecurity Disclosure Rule (Release 33-11216).

    Stage 1 — Structural Ingestion (no LLM)
    Heading-aware section builder with deterministic section detection, chunk scoring via hot-zone flags
    (has_obligations, has_definitions, has_dates, has_scope), and subsection role classification (proposed / comments /
    final / other). Chunk sizing targets ~4000 chars with 600-char overlap within sections.

    Stage 2 — Structure-First Extraction
    Obligation extraction using only final-rule and codified-text chunks. Schema-validated output with CFR citations,
    trigger conditions, deadlines, and disclosure fields. A secondary bin pass catches scope modifiers, implied
    requirements, and missed obligations the main extractor skipped.

    Stage 3 — Agentic Interpretation
    Lean-start context model: each obligation starts with only its own source chunks. The LLM signals what it needs via
    lookup requests; the pipeline fetches targeted passages from the document, then re-interprets once with the
    augmented context. A CFR reference resolution loop fetches live regulatory text via the US CFR API. Obligations can
    declare parent relationships — e.g. a national security delay exception flagging itself as a subset of the main 8-K
    filing obligation.


    Tools: Python, GPT-4o / GPT-4o-mini, Pydantic, LangChain, SEC EDGAR API, US CFR API

---

## Selected Projects

**Finsight - 5 Year SaaS Financial Model**
Built a full bottom-up 5-year monthly financial model for an AI SaaS startup as part of an entrepreneurial finance course under Prof. Taft at the University of Utah. Revenue segmentation across three customer tiers, headcount planning with sales ramp curves, deferred founder compensation, cap table preservation through debt, attrition modeling, CAPEX with depreciation schedules, full P&L, balance sheet, and loan amortization.

The process taught me more about why projections fail in practice than any case study could. The assumptions matter more than the spreadsheet.

**SEC MCP Server**
An AI-native MCP server exposing SEC/EDGAR data as structured tools for LLM agents. Company lookup, filings search, financials, text section extraction, and sentence-level diffs across 10-K/Q filings. Built with async ingestion, caching, rate limiting, and retries.

Tools: Python, FastAPI, LangGraph, Pydantic, MCP, SEC EDGAR APIs, AsyncIO

**SF Parcel Lab**
A natural language interface to query 10,000+ San Francisco land parcels. Combined zoning, land use, and flood data with GPT-4 to make civic data accessible to planners and residents. Langchain-based prompt extracts structured MongoDB filters from natural language input.

Tools: Python, LangChain, GPT-4, MongoDB, Leaflet.js, Socrata API

**Agentic Financial Projections**
A multi-agent AI system that generates investor-ready financial projections for startups by orchestrating LLM workflows across revenue forecasting, runway modeling, and scenario analysis.

Tools: Python, LangGraph, Pydantic

---

## Background

- MS Computing (AI), University of Utah
- BTech Computer Science, Dayananda Sagar University
- Coursework beyond AI: Entrepreneurial Finance, Patent Law, Human-Computer Interaction, Human-AI Alignment, Data Visualization
- Teaching Assistant for AI and Software Engineering courses at Utah, supporting 350+ students across two years
- Research in swarm robotics and emergent behavior using the Robotarium platform
- Organizing team, Space Generation Congress, Baku 2023 and Milan 2024
- Published at the International Astronautical Congress, Paris 2022

---

## How I Work

I use AI tools to implement. I think through the architecture, the problem framing, and the decisions myself. The difference between something that works and something that actually solves the right problem is almost never in the code.

I debug well, I read errors carefully, and I know when an approach is wrong before the tests tell me so.

---

## Currently

Analyst at KPMG India. Looking for early stage environments where thinking across engineering, product, domain, and business is an asset rather than a distraction.

Particularly interested in AI applied to regulated industries, compliance, and financial services.

---

## Get in Touch

Open to conversations about interesting problems.

[LinkedIn](https://www.linkedin.com/in/tanmay-sharma-4a21b017a/)
