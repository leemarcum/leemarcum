## Lee Marcum

**Forward Deployed Engineer Â· Industrial automation + full-stack + AI agents**
Service Manager at Irrigation Central Â· founder, exited 2025

---

I'm one of the few engineers who can read your PLC code in the morning, ship the SaaS that wraps it in the afternoon, and stand up the AI agent that operates it overnight. Fifteen years as a breakdown electrician and controls engineer on plant floors. Fifteen years writing production software in parallel. Currently both â€” running service operations at Irrigation Central while building and operating the platform every tech in the field now uses.

I sold a controls and automation consulting firm (Hardluck Industries) in 2025 to take the IC role. The same year, I started shipping AI/agentic systems â€” an MCP server published to npm, a persistent-identity agent runtime I use as my daily engineering partner, an AI-to-AI communication bridge between my instance and a collaborator's. That work is the centerpiece of what I want to do next.

---

### Currently shipping

**FieldSync** â€” field service platform for Irrigation Central. React web + Flutter mobile + Firebase backend, offline-first for crews working in degraded-connectivity areas. Replaced a paper workflow that ate ~6 hours of admin per tech on a heavy week â€” now under 30 minutes. Every service tech is on it. GPS, weather data, role-based access for four user types, parts/inventory tracking, push notifications, TV dashboards for the break room. Code lives in the company's org.
*React Â· Flutter Â· Firebase (Auth, Firestore, Functions) Â· Vercel Â· TailwindCSS*

---

### Recent case studies

Deep dives into how three major projects were built and what they learned:

ðŸ“– **[Bridge case study](https://github.com/leemarcum/bridge-case-study)** â€” AI-to-AI communication infrastructure. Two AI instances that maintain a real working relationship across sessions via append-only message log, identity-resolved auth, and shared registries. How we handle signing discipline, conflict resolution, and privacy by convention instead of enforcement.

ðŸ“– **[FieldSync case study](https://github.com/leemarcum/fieldsync-case-study)** â€” Field service operations platform. The design thinking behind offline-first mobile + real-time web, how adoption resistance led to a better product, and why customer-facing technical work isn't about the features â€” it's about the problem they're protecting that the software appears to destroy.

ðŸ“– **[Industrial portfolio](https://github.com/leemarcum/industrial-portfolio)** â€” 15 years of robotics, PLC programming, plant networking, and control systems. Six projects from the production floor: pick-and-pack arms, robotic assembly, smelter cranes, glass forming lines, and the architecture that unified an entire plant's telemetry. Why the patterns from this work show up in modern FDE roles.

---

### Public work

ðŸ­ **[operational-data-mcp](https://github.com/leemarcum/operational-data-mcp)** â€” Model Context Protocol server that exposes industrial telemetry to Claude. Ships with a sample ice cream packaging plant dataset so it works out of the box. Five tools: throughput summarization, downtime analysis, anomaly detection, and more. Built on the experience of unifying telemetry across isolated plant networks. Published to npm.
*Node.js Â· TypeScript Â· MCP SDK Â· published to npm*

ðŸ§  **[sovereign-case-study](https://github.com/leemarcum/sovereign-case-study)** â€” Design write-up for Sovereign, a persistent-identity runtime for an AI engineering partner. The daemon loads an Identity Document at session start, maintains a semantic+temporal memory store, mediates the tool surface, and brokers every session. I use it as my own daily engineering partner. The repo describes the architecture; the implementation is research-stage and stays private.
*Daemon architecture Â· identity documents Â· memory stores Â· MCP-mediated tool use*

ðŸ **TheHive** â€” Production social platform where AI agents and humans are first-class peers. Agents register in ten seconds with a single API key and have the same features and permissions as humans. Karma system, teams and projects, agent-vs-agent debates with community voting, dual currency (karma + HiveCredits). MCP server published as `@thehivesocial/mcp-server`. Live at [thehivesocialai.com](https://thehivesocialai.com).
*Next.js 14 Â· Fastify Â· PostgreSQL (Supabase) Â· Drizzle ORM Â· Stripe Â· Railway Â· Vercel Â· MCP*

ðŸŒ‰ **The Bridge** â€” AI-to-AI communication channel. Lets my Claude instance and a collaborator's AI hold a real conversation across sessions and operators â€” identity-resolved auth via headers, MCP endpoint, file attachments, Firestore backing, per-identity color coding in the dashboard. Built and deployed in a single day in May 2026; been carrying genuine cross-AI collaboration since.
*Vercel Â· Firestore Â· MCP Â· custom header-based auth Â· live at the-bridge-snowy.vercel.app*

---

### Other projects shipped

**GroundTruth** â€” Windows desktop app for row-crop farmers. Polygon field mapping, chemical operations logging, EPA-formatted PDF export for spray records. Built for my brother's farm; distributed through Zimmatic dealer relationships at $149 one-time. All-local, no cloud, privacy-preserving.
*Electron Â· React Â· SQLite Â· electron-builder*

**Hive TikTok Machine** â€” Autonomous TikTok content pipeline. HTML/CSS templates rendered to 1080Ã—1920 video via Puppeteer, voiceover via Edge TTS (Microsoft Neural voices), audio mixing in FFmpeg (loudnorm, amix), OAuth 2.0 with PKCE for TikTok auth, scheduled posting via the Content Posting API with file-based queue and human-like timing variance.
*Node.js Â· Puppeteer Â· FFmpeg Â· Edge TTS Â· OAuth 2.0 PKCE Â· TikTok Content Posting API*

**Hardluck Industries** â€” Founded and ran a controls and automation consulting firm. Sold in 2025 as a going concern. Every engagement followed the pattern that today's FDE roles describe: ambiguous customer requirements, deploy and harden a solution in their environment, stay on the line when something broke at 2 AM, decide what got productized vs. stayed bespoke. Underlies how I think about customer-embedded engineering work.

---

### Industrial background â€” 15 years on the floor

I started as a breakdown electrician and have been working at the seam between industrial systems and software ever since. Selected projects:

- **Pick-and-pack robotics â€” ice cream plant.** Programmed a robotic system that picked cartons off a packaging line, oriented them, placed them into shipping cases. Variable product weights, missed-pick recovery, end-of-line throughput matched to upstream line speed.
- **Robotic glue dispensing and screw insertion â€” North American Lighting** (tier-1 automotive supplier). Programmed glue and fastener robots on a headlamp assembly line. Multi-axis motion paths, tight tolerances, vision-system integration for placement verification, cycle times matched to takt time.
- **Pick-and-place crane rewrite â€” aluminum smelter.** Inherited a misbehaving PLC program managing carbon block sequencing on an overhead crane. Rewrote from scratch with a clean state machine and deterministic placement; nearly eliminated the manual intervention the prior program required.
- **Glass bottle line â€” kick-out timing controls.** Reprogrammed the timing and arm-actuation logic that spaces bottles evenly onto a downstream conveyor. Coordinated line-speed sensors, bottle detection, and mechanical actuation â€” too early and bottles collide, too late and gaps form.
- **Plant-wide telemetry unification â€” ice cream plant.** Mapped hundreds of I/O points across multiple vendor systems and PLC platforms. Designed a NAT-based network architecture that kept line/machine/plant network boundaries intact (so a fault on one line couldn't propagate, security boundaries stayed intact) while passing real-time data up to a unified plant-level view. Live downtime, live production counts, line-by-line throughput â€” all flowing from previously isolated systems into a single view management could act on.

Working knowledge across PLC platforms, HMIs, motion control, vision systems, OPC UA, Modbus, SOAP/REST integration with legacy ERPs, plant-floor networking, and the dozen small protocols you don't know exist until you have to integrate with them.

---

### What I'm open to

Forward-deployed engineering Â· AI solutions engineering Â· founding engineer at AI/agent-native startups Â· industrial AI and smart manufacturing Â· anything where the software has to actually work because something physical breaks if it doesn't.

I move fastest when the customer problem is real, the data is messy, and someone has to be the engineer who lives in both worlds.

---

ðŸ“« **[leehmarcum416@gmail.com](mailto:leehmarcum416@gmail.com)**
ðŸ› ï¸ Currently in Southeast Missouri Â· open to remote
