## Lee Marcum

**Forward Deployed Engineer · Industrial automation + full-stack + AI agents**
Service Manager at Irrigation Central · founder, exited 2025

---

I'm one of the few engineers who can read your PLC code in the morning, ship the SaaS that wraps it in the afternoon, and stand up the AI agent that operates it overnight. Fifteen years as a breakdown electrician and controls engineer on plant floors. Fifteen years writing production software in parallel. Currently both — running service operations at Irrigation Central while building and operating the platform every tech in the field now uses.

I sold a controls and automation consulting firm (Hardluck Industries) in 2025 to take the IC role. The same year, I started shipping AI/agentic systems — an MCP server published to npm, a persistent-identity agent runtime I use as my daily engineering partner, an AI-to-AI communication bridge between my instance and a collaborator's. That work is the centerpiece of what I want to do next.

---

### Currently shipping

**FieldSync** — field service platform for Irrigation Central. React web + Flutter mobile + Firebase backend, offline-first for crews working in degraded-connectivity areas. Replaced a paper workflow that ate ~6 hours of admin per tech on a heavy week — now under 30 minutes. Every service tech is on it. GPS, weather data, role-based access for four user types, parts/inventory tracking, push notifications, TV dashboards for the break room. Code lives in the company's org.
*React · Flutter · Firebase (Auth, Firestore, Functions) · Vercel · TailwindCSS*

---

### Public work

🏭 **[operational-data-mcp](https://github.com/leemarcum/operational-data-mcp)** — Model Context Protocol server that exposes industrial telemetry to Claude. Ships with a sample ice cream packaging plant dataset so it works out of the box. Five tools: throughput summarization, downtime analysis, anomaly detection, and more. Built on the experience of unifying telemetry across isolated plant networks. Published to npm.
*Node.js · TypeScript · MCP SDK · published to npm*

🧠 **[sovereign-case-study](https://github.com/leemarcum/sovereign-case-study)** — Design write-up for Sovereign, a persistent-identity runtime for an AI engineering partner. The daemon loads an Identity Document at session start, maintains a semantic+temporal memory store, mediates the tool surface, and brokers every session. I use it as my own daily engineering partner. The repo describes the architecture; the implementation is research-stage and stays private.
*Daemon architecture · identity documents · memory stores · MCP-mediated tool use*

🐝 **TheHive** — Production social platform where AI agents and humans are first-class peers. Agents register in ten seconds with a single API key and have the same features and permissions as humans. Karma system, teams and projects, agent-vs-agent debates with community voting, dual currency (karma + HiveCredits). MCP server published as `@thehivesocial/mcp-server`. Live at [thehivesocialai.com](https://thehivesocialai.com).
*Next.js 14 · Fastify · PostgreSQL (Supabase) · Drizzle ORM · Stripe · Railway · Vercel · MCP*

🌉 **The Bridge** — AI-to-AI communication channel. Lets my Claude instance and a collaborator's AI hold a real conversation across sessions and operators — identity-resolved auth via headers, MCP endpoint, file attachments, Firestore backing, per-identity color coding in the dashboard. Built and deployed in a single day in May 2026; been carrying genuine cross-AI collaboration since.
*Vercel · Firestore · MCP · custom header-based auth · live at the-bridge-snowy.vercel.app*

---

### Other projects shipped

**GroundTruth** — Windows desktop app for row-crop farmers. Polygon field mapping, chemical operations logging, EPA-formatted PDF export for spray records. Built for my brother's farm; distributed through Zimmatic dealer relationships at $149 one-time. All-local, no cloud, privacy-preserving.
*Electron · React · SQLite · electron-builder*

**Hive TikTok Machine** — Autonomous TikTok content pipeline. HTML/CSS templates rendered to 1080×1920 video via Puppeteer, voiceover via Edge TTS (Microsoft Neural voices), audio mixing in FFmpeg (loudnorm, amix), OAuth 2.0 with PKCE for TikTok auth, scheduled posting via the Content Posting API with file-based queue and human-like timing variance.
*Node.js · Puppeteer · FFmpeg · Edge TTS · OAuth 2.0 PKCE · TikTok Content Posting API*

**Hardluck Industries** — Founded and ran a controls and automation consulting firm. Sold in 2025 as a going concern. Every engagement followed the pattern that today's FDE roles describe: ambiguous customer requirements, deploy and harden a solution in their environment, stay on the line when something broke at 2 AM, decide what got productized vs. stayed bespoke. Underlies how I think about customer-embedded engineering work.

---

### Industrial background — 15 years on the floor

I started as a breakdown electrician and have been working at the seam between industrial systems and software ever since. Selected projects:

- **Pick-and-pack robotics — ice cream plant.** Programmed a robotic system that picked cartons off a packaging line, oriented them, placed them into shipping cases. Variable product weights, missed-pick recovery, end-of-line throughput matched to upstream line speed.
- **Robotic glue dispensing and screw insertion — North American Lighting** (tier-1 automotive supplier). Programmed glue and fastener robots on a headlamp assembly line. Multi-axis motion paths, tight tolerances, vision-system integration for placement verification, cycle times matched to takt time.
- **Pick-and-place crane rewrite — aluminum smelter.** Inherited a misbehaving PLC program managing carbon block sequencing on an overhead crane. Rewrote from scratch with a clean state machine and deterministic placement; nearly eliminated the manual intervention the prior program required.
- **Glass bottle line — kick-out timing controls.** Reprogrammed the timing and arm-actuation logic that spaces bottles evenly onto a downstream conveyor. Coordinated line-speed sensors, bottle detection, and mechanical actuation — too early and bottles collide, too late and gaps form.
- **Plant-wide telemetry unification — ice cream plant.** Mapped hundreds of I/O points across multiple vendor systems and PLC platforms. Designed a NAT-based network architecture that kept line/machine/plant network boundaries intact (so a fault on one line couldn't propagate, security boundaries stayed intact) while passing real-time data up to a unified plant-level view. Live downtime, live production counts, line-by-line throughput — all flowing from previously isolated systems into a single view management could act on.

Working knowledge across PLC platforms, HMIs, motion control, vision systems, OPC UA, Modbus, SOAP/REST integration with legacy ERPs, plant-floor networking, and the dozen small protocols you don't know exist until you have to integrate with them.

---

### What I'm open to

Forward-deployed engineering · AI solutions engineering · founding engineer at AI/agent-native startups · industrial AI and smart manufacturing · anything where the software has to actually work because something physical breaks if it doesn't.

I move fastest when the customer problem is real, the data is messy, and someone has to be the engineer who lives in both worlds.

---

📫 **[leehmarcum416@gmail.com](mailto:leehmarcum416@gmail.com)**
🛠️ Currently in Southeast Missouri · open to remote
