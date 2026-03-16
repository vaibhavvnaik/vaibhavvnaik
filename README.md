# Hey, I'm Vaibhav 👋

**builder turned PM — shipping at the intersection of Developer Platforms, API Management, AI Agents, and deal discovery.**

PM at Remitly, VMWare..

---

## 🔨 What I'm Building

### [urklist.com](https://urklist.com) — AI-Native Deal Discovery Platform

A promotional email aggregation platform that consolidates retail brand newsletters into a unified, filterable feed. The emails are the data source — the deals are the product.

- **Problem:** Deals, promo codes, and sale alerts get buried across dozens of brand newsletters. Consumers miss promotions; brands lose engagement.
- **Solution:** An autonomous agent subscribes to brand newsletters, captures every email, extracts deal content, and surfaces it in a browsable, category-first feed at [urklist.com](https://urklist.com).
- **Categories:** 15+ verticals — Grocery, Footwear, Clothing, Home, Electronics, Travel, Restaurants, Beauty, Health, Sports, Kids, Pets, and more.
- **Stack:** Next.js 13 · TypeScript · Tailwind · NextAuth · Prisma · MongoDB · Vercel

### [brand-onboarding-agent](https://github.com/vaibhavvnaik/brand-onboarding-agent) — Autonomous Newsletter Ingestion Pipeline

The backend engine powering urklist's content supply. Discovers brands, signs up for newsletters via browser automation, processes confirmation emails, and ingests newsletter content — all autonomously.

- **Browser Automation:** Playwright with 40+ CSS selector patterns across Mailchimp, Klaviyo, Substack, Shopify, and custom signup forms
- **Pipeline:** discover_and_signup → scan_inbox → process_confirmations → ingest_newsletters
- **Stack:** Node.js · Express · MongoDB · Playwright · Gmail API · Ollama LLM · Backblaze B2 · Railway · Docker

### [brand-onboarding-agent-agentic](https://github.com/vaibhavvnaik/brand-onboarding-agent-agentic) — Production AI Agent with Memory, Self-Healing & Orchestration

The evolved agentic version of the pipeline — implements 7 production-grade AI agent patterns that go beyond basic prompt-and-respond:

- **LLM Planner** with heuristic fallback — decides which stage to run next based on queue state and memory context
- **3-Level Persistent Memory** — semantic (cross-run tool reliability), episodic (300-entry sliding window + incident learning), per-run (crash recovery checkpoints)
- **7 Specialized Sub-Agents** — coordinated by the planner, each handling a distinct pipeline capability
- **Human-in-the-Loop (HITL)** — configurable approval gates on high-risk operations with SSE event emission
- **Self-Healing** — 6 failure categories (CAPTCHA, selector breakage, timeout, rate limit, runtime dependency, LLM parse error) with auto-recovery routing
- **Observability** — SSE live streaming, run quality scoring (0–100 composite), diagnostic endpoints, evaluation framework
- **MCP Integration** — Model Context Protocol for external tool extensibility and browser automation handoff

### [ChatGPT GPT — Interactive Demo](https://chatgpt.com/g/g-69b7434270ac8191bffbc5d8ac9cb147-brand-onboarding-newsletters-ingestion-agent)

A custom ChatGPT GPT that serves as a conversational interface to explore the agent architecture, urklist.com's product strategy, and the agentic patterns — backed by detailed knowledge bases.

---

## 🧠 How I Think About Product

- **Reduce activation energy** — if a user has to think about it, it's already too complex
- **Data as UX** — the best features come from treating unstructured content (emails, links, newsletters) as structured, queryable data
- **Build the supply side first** — automate content acquisition before optimizing consumption. The agent feeds the platform.
- **Measure then cut** — every feature starts as a hypothesis; shipping is how you find out if it's true

---

## 🗺️ What's Next

- AI-powered promo code extraction and deal scoring
- Price drop alerts and category-level deal comparison
- Affiliate monetization and Urklist Pro subscription tier
- SMS/push notification tracking — a channel nobody archives yet
- Public API for developers

---

## 📬 Let's Connect

- 💼 [LinkedIn](https://linkedin.com/in/vaibhavvnaik)

---

*PM · Solo Builder · AI Agents · Deal Discovery · Developer Platforms · API Management · he/him*
