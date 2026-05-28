# David Fernández Morilla

Independent developer based in Vigo, Spain. I build products, operate their infrastructure and find security flaws along the way.

Six published CVEs on WordPress plugins under the **NyxSec** handle (Wordfence advisories on Elementor, WPForms, Masteriyo LMS, Bookit and Five Star Restaurant Reservations). Multi-agent systems with LLM cost telemetry per pipeline. Production platforms running on self-managed infra (VPS, AWS, K3s, Docker).

→ **Full work and case studies:** [davidfdzmorilla.dev](https://davidfdzmorilla.dev)

---

### Pinned

The four projects below are the public ones. Most of my active work is closed source but lives in production: the bug bounty pipeline, [kaleido](https://kaleidostudio.davidfdzmorilla.dev) (multi-channel conversational platform), [wedding](https://wedding.davidfdzmorilla.dev) (multi-tenant wedding SaaS), [gofestivals](https://gofestivals.es) (electronic music festivals platform), and a multi-agent orchestration ecosystem. The portfolio covers everything.

**[radio-gofestivals](https://github.com/davidfdzmorilla/radio-gofestivals)** — Curated electronic music radio platform. 1,300+ stations across 12 genres with multi-stream auto-fallback, hybrid auth (anonymous favorites + optional sync), real-time spectrum analyzer. FastAPI + Postgres + Redis + Next.js 14, ICY metadata worker. Live at [radio.gofestivals.eu](https://radio.gofestivals.eu).

**[tech-blog](https://github.com/davidfdzmorilla/tech-blog)** — Autonomous media platform with 9 specialized AI agents communicating via Redis event bus. 8-stage pipeline (discovery → trends → editorial → research → writing → review → SEO → publish), Chief Editor as quality gatekeeper, semantic dedup via Qdrant, LLM cost telemetry per pipeline run. FastAPI + Next.js 14 + PostgreSQL + Qdrant. Live at [techblog.davidfdzmorilla.dev](https://techblog.davidfdzmorilla.dev).

**[pharmacy-recommendation-system](https://github.com/davidfdzmorilla/pharmacy-recommendation-system)** — Smart pharmacy POS for Raspberry Pi 4. USB barcode scanner feeds a Claude Sonnet 4 recommendation engine that suggests therapeutic complements based on the full cart (gastric protectors with NSAIDs, probiotics with antibiotics, etc). LRU + TTL caching keeps cached responses under 100ms. SQLite + tkinter + Docker for development on Mac via XQuartz.

**[chatbot-whatsapp](https://github.com/davidfdzmorilla/chatbot-whatsapp)** — WhatsApp AI chatbot built with Clean Architecture and DDD. Claude Sonnet 4 via Anthropic API + Twilio WhatsApp + PostgreSQL (Prisma) + Redis for context cache. TypeScript strict mode, structured logging with Winston, Helmet + rate limiting, Jest test suite.

---

### Reach

[davidfdzmorilla.dev](https://davidfdzmorilla.dev) · [LinkedIn](https://www.linkedin.com/in/davidfdzmorilla/) · correo@davidfdzmorilla.dev
