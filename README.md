# Ben Milch

**Senior Product & Program Manager — I build the tooling instead of writing a spec and waiting on engineering.**

A decade-plus in financial-services product and program work across Big 4 consulting (PwC, Accenture, EY, Deloitte) — compliance, fraud, AML/KYC, and Web3 programs for clients including Morgan Stanley, Capital One, Citi, and Wells Fargo. In parallel, 27 years running an e-commerce business with full P&L. Today I operate as an **AI-orchestrated power user**: I design and ship data pipelines, AI integrations, and operational tooling directly, without a dedicated engineering team.

### Things I've built

- **A self-monitoring, self-healing operations estate** — single-operator monitoring with bounded auto-remediation (it will never restart a database or a node — enforced in code), rolling uptime/MTTR history with no database, a zero-dependency public status page, and a DR toolkit whose git backup *aborts if it would leak a secret*. Open-sourced from the running deployment. → [estate-sentinel](https://github.com/benmilch-eth/estate-sentinel)
- **Multi-provider AI failover** — ordered failover across LLM providers so no single vendor outage can take the automation down; raises only when every provider fails, with every provider's error in the exception. One file, MIT. → [llm-failover](https://github.com/benmilch-eth/llm-failover)
- **Blockchain-anchored media authentication** — an Ed25519 device-signing client, on-chain anchoring of signature commitments to Ethereum (Sepolia), and a listener + verifier that produce verifiable provenance receipts. Ships with a threat model. → [media-auth](https://github.com/benmilch-eth/media-auth)
- **A one-person AI "organization"** — standing agent threads that coordinate *asynchronously, by writing each other letters*, moved by a small set of scheduled "mailroom" agents. Stateless per run, fully auditable, human-in-the-loop. → [ai-orchestration-kit](https://github.com/benmilch-eth/ai-orchestration-kit)
- **Computer-vision cataloging** — a Claude Vision pipeline that turns a single photograph into a marketplace-ready listing (title, condition grade, price range, confidence flags) at roughly $0.014 per item. → [claude-vision-cataloger](https://github.com/benmilch-eth/claude-vision-cataloger)
- **An AI-operated collectibles business** — end to end: it sources undervalued vintage cards across marketplaces, prices them against real graded sold-comps, predicts grading arbitrage from card scans, and matches each find to the individual buyer most likely to want it — scored on era, grade tier, player, and price against deep purchase-history profiles of **16,000+ buyers**, and gated on net profit *after* real shipping and handling so it never surfaces a $5 deal. A public intake at [sell.sportscardsforever.com](https://sell.sportscardsforever.com) turns any consignor's list — spreadsheet, dealer PDF, or phone photos — into a comp-backed cash offer within the quarter hour. Every offer and buyer message is drafted for a human to approve; nothing auto-sends.
- **Data infrastructure** — Azure SQL forensic diagnosis across 100K+ rows; ETL and backfill pipelines; production integrations against the Gmail, ShipStation, and Discogs APIs.
- **Web3** — Solidity (Cyfrin Updraft); tokenization and wallet-services strategy at Accenture, including NFT product work for Amazon and the Golden State Warriors.

### How I think about building

Async over real-time. Drafts over autonomous actions — the human stays on the consequential calls. Flagged, never auto-resolved: every judgment call routes to a named human with full context. Single sources of truth over tribal memory. A cheap check before every expensive job. Boring, auditable, and trustworthy beats clever.

### Toolbelt

Python · Azure SQL / SQL Server · Claude & GPT APIs · Playwright · scheduled-agent orchestration · SQL-first data work

### Elsewhere

- LinkedIn — <https://www.linkedin.com/in/benjaminmilch>
- Writing on AI orchestration — <https://substack.com/@benmilch>
- 🖥️ **Live:** my always-on AI operation — **60+ automated systems, self-hosted, with public uptime/MTTR** → [ops.benmilch.com](https://ops.benmilch.com)
