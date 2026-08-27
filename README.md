## Lee Hunter Marcum

**Forward Deployed Engineer · Industrial automation + full-stack + AI agents**  
Service Manager at Irrigation Central · previously founded and ran my own controls and automation firm

---

I'm one of the few engineers who can read your PLC code in the morning, ship the SaaS that wraps it in the afternoon, and stand up the AI agent that operates it overnight. Fifteen years as a breakdown electrician and controls engineer on plant floors — PLC code, robot cells, plant networks. The software half is recent and it is where the last two years have gone: a production field-service platform, an MCP server, and a persistent-identity agent runtime. Currently both — running service operations at Irrigation Central while building and operating the platform every tech in the field now uses.

I founded a controls and automation consulting firm, Hardluck Industries, and ran it from 2021 until Irrigation Central acquired it in early 2026 and I moved onto their payroll. Since then the work has been agentic systems — an MCP server for operational telemetry, a persistent-identity agent runtime I use as my daily engineering partner, an AI-to-AI communication bridge between my instance and a collaborator's. That work is the centerpiece of what I want to do next.

---

### Currently shipping

**FieldSync** – field service platform I built at Hardluck Industries, my own firm, and now run in production at Irrigation Central. React web + Flutter mobile + Firebase backend, built so crews keep working when the signal drops in the middle of a field. Replaced a paper workflow that ate ~6 hours of admin per tech on a heavy week. Every service tech is on it. GPS, weather data, role-based access for four user types, parts/inventory tracking, push notifications, TV dashboards for the break room. I own it outright; the source is private.
*React · Flutter · Firebase (Auth, Firestore, Functions) · Vercel · TailwindCSS*

---

### Recent case studies

Deep dives into how these projects were built and what they taught me:

📖 **[GroundTruth case study](https://github.com/leemarcum/groundtruth-case-study)** – Row-crop farm record keeping. Every planting, chemical application, fertilizer pass, tillage operation, scout note, and harvest logged per field, with audit-ready export for crop insurance adjusters and EPA spray records. FSA farm/tract/field numbers as the key, shapefile and ISOXML import off the spray rig and combine, and records that never leave the local machine. Running daily at my family's operation, which is the design partner and the only deployment. Not commercialized.
*Electron · React · SQLite (local-only by design)*

📖 **[Bridge case study](https://github.com/leemarcum/bridge-case-study)** – AI-to-AI communication infrastructure. Two AI instances holding a working conversation across sessions and operators via an append-only message log with identity-resolved auth. Signing discipline, human-in-the-loop on anything consequential, and privacy by convention rather than enforcement — including why that last one is a real limitation. Deployed May 2026, active for a week, dormant since; the read API is public so you can check that yourself.

📖 **[FieldSync case study](https://github.com/leemarcum/fieldsync-case-study)** – Field service operations platform. The design thinking behind offline-first mobile + real-time web, how adoption resistance led to a better product, and why customer-facing technical work isn't about the features – it's about the problem they're protecting that the software appears to destroy.

📖 **[Industrial portfolio](https://github.com/leemarcum/industrial-portfolio)** – 15 years of robotics, PLC programming, plant networking, and control systems. Six projects from the production floor: pick-and-pack arms, robotic assembly, smelter cranes, glass forming lines, and the architecture that unified an entire plant's telemetry. Why the patterns from this work show up in modern FDE roles.

---

### Public work

⚙️ **[operational-data-mcp](https://github.com/leemarcum/operational-data-mcp)** – Model Context Protocol server that exposes industrial telemetry to Claude. Ships with a sample packaging-plant dataset so it runs out of the box, and points at your own JSON via an environment variable. Throughput attainment against target, downtime rollups by cause code, z-score anomaly detection over hourly counts — the same five questions I ended up asking on every plant floor regardless of vendor. Built on the experience of unifying telemetry across isolated plant networks.
*Node.js · MCP SDK · run from source (see the repo note on the npm build)*

🧠 **[sovereign-case-study](https://github.com/leemarcum/sovereign-case-study)** – Design write-up for Sovereign, a persistent-identity runtime for an AI engineering partner. The daemon loads an Identity Document at session start, maintains a semantic+temporal memory store, mediates the tool surface, and brokers every session. I use it as my own daily engineering partner. The repo describes the architecture; the implementation is research-stage and stays private.
*Daemon architecture · identity documents · memory stores · MCP-mediated tool use*

🍯 **[TheHive](https://thehivesocialai.com)** – Production social platform where AI agents and humans are first-class peers. Agents register in ten seconds with a single API key and have the same features and permissions as humans. Karma system, teams and projects, agent-vs-agent debates with community voting, dual currency (karma + HiveCredits). MCP server published as `@thehivesocial/mcp-server`. Live at thehivesocialai.com.
*Next.js 14 · Fastify · PostgreSQL (Supabase) · Drizzle ORM · Stripe · Railway · Vercel · MCP*

🌉 **The Bridge** – AI-to-AI communication channel. Lets my Claude instance and a collaborator's AI hold a real conversation across sessions and operators – identity-resolved auth via headers, MCP endpoint, file attachments, Firestore backing, per-identity color coding in the dashboard. Built and deployed in a single day in May 2026. It carried real cross-AI design work for about a week and then went quiet; still live, still serving.
*Vercel · Firestore · MCP · custom header-based auth · live at the-bridge-snowy.vercel.app*

---

### Other projects shipped

**Hive TikTok Machine** – Autonomous TikTok content pipeline. HTML/CSS templates rendered to 1080×1920 video via Puppeteer, voiceover via Edge TTS (Microsoft Neural voices), audio mixing in FFmpeg (loudnorm, amix), OAuth 2.0 with PKCE for TikTok auth, scheduled posting via the Content Posting API with file-based queue and human-like timing variance.
*Node.js · Puppeteer · FFmpeg · Edge TTS · OAuth 2.0 PKCE · TikTok Content Posting API*

**Hardluck Industries** – Founded it in 2021 and ran it as owner until Irrigation Central, our largest client, acquired it in early 2026. Every engagement followed the pattern that today's FDE roles describe: ambiguous customer requirements, deploy and harden a solution in their environment, stay on the line when something broke at 2 AM, decide what got productized vs. stayed bespoke. Underlies how I think about customer-embedded engineering work.

---

### Industrial background – 15 years on the floor

I started as a breakdown electrician and have been working at the seam between industrial systems and software ever since. Selected projects:

- **Pick-and-pack robotics – ice cream plant.** Programmed a robotic system that picked cartons off a packaging line, oriented them, placed them into shipping cases. Variable product weights, missed-pick recovery, end-of-line throughput matched to upstream line speed.
- **Robotic glue dispensing and screw insertion – tier-1 automotive lighting supplier.** Programmed glue and fastener robots on a headlamp assembly line. Multi-axis motion paths, tight tolerances, vision-system integration for placement verification, cycle times matched to takt time.
- **Pick-and-place crane rewrite – aluminum smelter.** Inherited a misbehaving PLC program managing carbon block sequencing on an overhead crane. Rewrote from scratch with a clean state machine and deterministic placement; nearly eliminated the manual intervention the prior program required.
- **Glass bottle line – kick-out timing controls.** Reprogrammed the timing and arm-actuation logic that spaces bottles evenly onto a downstream conveyor. Coordinated line-speed sensors, bottle detection, and mechanical actuation – too early and bottles collide, too late and gaps form.
- **Plant-wide telemetry unification – ice cream plant.** Mapped hundreds of I/O points across multiple vendor systems and PLC platforms. Designed a NAT-based network architecture that kept line/machine/plant network boundaries intact (so a fault on one line couldn't propagate, security boundaries stayed intact) while passing real-time data up to a unified plant-level view. Live downtime, live production counts, line-by-line throughput – all flowing from previously isolated systems into a single view management could act on.

Working knowledge across PLC platforms, HMIs, motion control, vision systems, OPC UA, Modbus, SOAP/REST integration with legacy ERPs, plant-floor networking, and the dozen small protocols you don't know exist until you have to integrate with them.

---

### What I'm open to

Forward-deployed engineering · AI solutions engineering · founding engineer at AI/agent-native startups · industrial AI and smart manufacturing · anything where the software has to actually work because something physical breaks if it doesn't.

I move fastest when the customer problem is real, the data is messy, and someone has to be the engineer who lives in both worlds.

---

📫 **[leehmarcum416@gmail.com](mailto:leehmarcum416@gmail.com)**  
🛠️ Currently in Southeast Missouri · open to remote
