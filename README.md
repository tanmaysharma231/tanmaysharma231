# Hi, I'm Tanmay Sharma

MS in Computing (AI) from the University of Utah. Based in Bangalore.

I tend to think across a lot of layers at once. That's why alongside my AI degree I studied entrepreneurial finance, patent law, and human-computer interaction. Not because I had to but because I was curious about how technology actually lands in the real world across business, legal, and human layers.

I'm more energized by figuring out what needs to be built and why than by implementing what's already been decided.

---

## What I'm Working On

**SEC Regulatory Document Interpreter**
A pipeline that takes raw SEC regulatory PDFs and produces structured obligations with CFR citations, then interprets each one using the SEC's own comment responses. The insight that drove it: extraction is not the hard part. Interpretation is. Figuring out what an obligation means operationally, what is ambiguous, and what a company actually needs to change is where the real difficulty lives.

Built and tested on the 2023 SEC Cybersecurity Disclosure Rule (Release 33-11216). Current approach uses structural document parsing to identify obligation sections deterministically before passing to an LLM, with a secondary fallback pass to catch scope modifiers and implied requirements.

- Stage 1: Structural ingestion with no LLM, heading detection, chunk scoring
- Stage 2: Structure-first obligation extraction with CFR citations and schema validation
- Stage 3: Interpretation using context bundles built from SEC comment responses and live CFR API data

Tools: Python, GPT-4o, Pydantic, SEC EDGAR API, US CFR API

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
