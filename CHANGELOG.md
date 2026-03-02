# The OpenClaw Bible — Changelog

> **Latest additions appear at the top.** Each entry includes a date, source, and link to the relevant section.

---

## 2026-03-02 (Density trim — ~150 lines cut)

### Updated
- **Ch 1, 2, 3, 4, 7, 8, 11, Appendix B** — Trimmed cross-chapter duplication and verbose explanations. Principle: "why & when to use it + one command" instead of "how it works in detail." Algorithm explanations → one-sentence summaries. Nested sub-agent/ACP/secrets sections in non-canonical chapters → brief mention + link. Minor providers in Ch 8 → flowing prose without sub-headers. Appendix B hardening fixes → category + count format. Net -151 lines.

---

## 2026-03-02 (Rename + parody intro)

### Updated
- **Renamed "The OpenClaw Guidebook" → "The OpenClaw Bible"** across all files (index, CLAUDE.md, CHANGELOG.md)
- **0. The OpenClaw Bible.md** — Added parody hook intro that roasts the timeline's engagement-bait OpenClaw threads and positions the Bible as the antidote to information overload

---

## 2026-03-02 (Guidebook overhaul — 2026.2.17 → 2026.3.1 update)

### Added
- **0. Bible Index** — "What's New in 2026.3.1" summary section with all major changes
- **2. Core Concepts** — Nested sub-agents, ACP thread-bound agents, MMR memory re-ranking, lifecycle status reactions, session cleanup CLI
- **3. Security** — "2026.3.1 Security Hardening" section (30+ fixes summary), external secrets management (`openclaw secrets`), minimum version recommendation
- **5. Use Cases** — Sub-agent orchestration, per-DM topic config, webhook-triggered workflows
- **8. Tools & Plugins** — Kilo Gateway, Volcano Engine/BytePlus, Kimi web search, Moonshot video, OpenAI WebSocket streaming
- **11. Multi-Agent Coordination** — Agent bindings (`openclaw agents bind/unbind`), ACP thread-bound agents, nested sub-agents (depth config, patterns), lifecycle status reactions, MMR re-ranking
- **Appendix A** — `openclaw secrets`, `openclaw sessions cleanup`, `openclaw agents bind/unbind`, `openclaw update` commands
- **Appendix B** — External secrets management template, 2026.3.1 security hardening bullet summary
- **Appendix C** — Agent bindings visualization, secrets rotation status

### Updated
- **0. Bible Index** — Updated chapter descriptions and quick reference table
- **1. Getting Started** — Android app, Gemini 3.1 + Kilo Gateway providers, external secrets in setup flow, Claude 4.6 adaptive thinking note
- **2. Core Concepts** — Adaptive thinking note in Brains & Muscles
- **4. Identity Files** — Nested sub-agent guidance in AGENTS.md, secrets security callout, adaptive thinking note
- **6. Life Automation** — Updated AI tool categories (Gemini 3.1, Moonshot video, sub-agent delegation)
- **7. Skills System** — Gemini model references updated, nested sub-agents in skills, external secrets for API keys
- **8. Tools & Plugins** — Gemini model references updated, external secrets tip
- **9. Cost Optimization** — Gemini 3.1 in tier table, Kilo Gateway routing, Claude 4.6 adaptive thinking costs, nested sub-agent costs
- **10. Content Curation** — Per-DM topic config, Android mobile capture
- **12. Marketing** — Android app mention, session cleanup for cost management, archived source file references

### Removed
- **Raw source files** — `vibe-marketing-raw.md`, `vibe-marketing-articles.md`, `openclaw-raw-scrapes.md`, `OpenClaw Extract.md` (content preserved in guidebook chapters)

### Moved
- **ACE_OpenClaw_Analysis.md** — Moved from `📱 Projects/🔧 OpenClaw/` to `📱 Projects/⚡ ACE/`

---

## 2026-03-02 (Community scrape — 9 tweets + GitHub repo)

### Updated
- **1. Getting Started** — Added auto-update config (off by default, JSON config to enable). Source: @ziwenxu_ https://x.com/ziwenxu_/status/2028358855780868188
- **2. Core Concepts & Architecture** — Added tiered memory with trust scoring (Constitutional/Strategic/Operational tiers, hit counts, supersede chains), active context holds (temporary filters with expiry), nightly extraction automation. Source: @AtlasForgeAI article https://x.com/AtlasForgeAI/status/2026380335249002843
- **4. Identity & Personality Files** — Added Voice DNA section (banned phrases, writing rules, writing samples for voice matching), meta-learning loops (regressions list, friction log, prediction-outcome calibration). Source: @itsolelehmann https://x.com/itsolelehmann/status/2028497454635888982, @AtlasForgeAI article
- **5. Use Cases & Workflows** — Added awesome-openclaw-usecases repo reference (34+ community use cases, 11K stars), animated video production use case, AI business ideas section (8 revenue-generating service models). Source: @Hesamation https://x.com/Hesamation/status/2027454736358903939, @Crypto_Jargon, @milesdeutscher https://x.com/milesdeutscher/status/2026225858281963741
- **8. Tools & Plugins** — Added Pinchtab (lightweight Go browser control), Electron skill for agent-browser (control desktop apps), Kepano's official Obsidian skills note. Source: @GithubProjects, @ctatedev https://x.com/ctatedev/status/2028128730132922760, @Hesamation

---

## 2026-02-25 (Twitter content strategy automation + new skills)

### Added
- **social-graph-audit.ts** — Weekly Monday script. Compares who you follow vs. who you've engaged with in the last 30 days. Uses Claude Haiku to surface 7 accounts worth reaching out to. Sends to Telegram. Cron: `30 9 * * 1`
- **engagement-radar.ts** — Weekly Friday script. Finds accounts that have been replying to/mentioning you that you haven't replied back to. Surfaces 5-7 warm leads to acknowledge. Cron: `30 9 * * 5`
- **tweet-pattern-report.ts** — Monthly script (1st of month). Analyzes your own tweet performance: topics, formats, what's working, one concrete recommendation. Sends to Telegram. Cron: `0 9 1 * *`
- **thread-weaver skill** — OpenClaw + Claude Code skill. Before writing any new thread, searches existing tweet archive for related threads to cross-reference. Builds the cinematic universe.
- **agentmail skill** — OpenClaw + Claude Code skill. Send/receive email via flawd@agentmail.to. API key wired up in global.env.
- **copywriting skill** — The Recursive Marketing Prompt. 7-reader × 3-failure-layer validation before showing copy to user.
- **skill-manager skill** — Auto-activates on skill install/create/remove requests. Enforces MetaBrain 3 paths.

### Source
- Visa (@visakanv) "How to Play Twitter" playbook — `📝 Notes/🌳 Life/How to Play Twitter.md`

---

## 2026-02-24 (Community insights — 15 threads + 2 articles)

### Updated
- **1. Getting Started** — Added advanced Discord channel setup (forum sessions, code RAG, shopping watchdog, music feedback loop). Source: @0xSero
- **2. Core Concepts & Architecture** — Added Mac launchd tip, Spark memory layer, OpenClaw vs n8n/Zapier table. Source: @cathrynlavery, @meta_alchemist, @wickedguro
- **3. Security & Hardening** — Added community hardening tips (6 points from ex-Cisco engineer). Source: @johann_sath
- **4. Identity & Personality Files** — Added SOUL.md directives, co-founder framing, nightly self-improvement loop, introspective prompting (9 prompts). Source: @johann_sath, @EXM7777, @nateliason, @kloss_xyz
- **5. Use Cases & Workflows** — Added use cases: Home Automation (Homey), Travel Assistant, Messages Intelligence (Beeper), Context-Aware Mode, Business Agent. Added prompts 12-16. Source: @nateliason article, @krausefx blog
- **7. Skills System** — Added skills-as-products framing, memory hygiene section. Source: @chrysb, @wickedguro
- **8. Tools & Plugins** — Added Scrapling, WisprFlow, OpenClaw Deck, Spark, agent-browser. Source: @hasantoxr, @itsolelehmann, @Austen, @meta_alchemist, @wickedguro
- **9. Cost Optimization** — Added Haiku for heartbeats tip with real-world routing from Felix. Source: @nateliason
- **11. Multi-Agent Coordination** — Added Sub-Agent Review Pattern, Main-Agent-as-Planner Pattern. Source: @EXM7777, @johann_sath
- **12. Marketing Automation** — Added TikTok Slideshow Growth Engine, Selling Skills as Products, CLI-First Tool Design. Source: @wickedguro article

---

## 2026-02-24

### Added
- **Chapter 12: Marketing Automation & Vibe Marketing** — Expanded comprehensive guide with 4 new major sections: (1) Advanced Agent Orchestration — agent teams for parallel marketing work; (2) Content Pipeline at Scale — real case study of 80+ articles published in 10 days ($0.70/article); (3) Marketing Supercomputer — build expert advisors trained on great marketers' content; (4) Vibe Marketing Framework & 22+ reusable skills library. Source: 10 in-depth articles from marketing automation practitioners (vibe-marketing-articles.md). Related: [[0. The OpenClaw Bible#Chapter 12]], [[CLAUDE.md#Chapter 12 Walkthrough Guide]]
- **vibe-marketing-raw.md** — Raw collection of 25 tweets from marketing automation practitioners. Full untruncated text from Twitter API v2. Engagement metrics: 41,674 total (39,041 likes + 2,633 retweets).
- **vibe-marketing-articles.md** — Full text of 10 reference articles with detailed case studies, implementation patterns, and real results from marketing automation in production.

### Updated
- **0. The OpenClaw Bible.md** — Added Chapter 12 to TOC and quick reference table
- **CLAUDE.md** — Added Chapter 12 walkthrough guide with setup actions
- **Chapter 12: Marketing Automation & Vibe Marketing** — Distilled and merged article insights. Added 4 major new sections covering agent orchestration, content pipelines, expert advisors, and 22+ skills library.

---

## 2026-02-18

### Added
- **CHANGELOG.md** — Created this changelog to track all future additions to the guidebook. New entries should always be added at the top.

---

## Template for New Entries

```markdown
## YYYY-MM-DD

### Added
- **[Topic/Feature Name]** — Brief description. Source: [Link or "Summarize plugin"]. Related: [[Chapter Name#Section]]

### Updated
- **[Topic/Feature Name]** — What changed and why.

### Fixed
- **[Topic/Feature Name]** — What was corrected.

```

---

## Legend

| Type | Meaning |
|------|---------|
| Added | New content, sections, or files |
| Updated | Changes to existing content |
| Fixed | Corrections or clarifications |

---

## Sources

When adding from the Summarize plugin, include:
- Original URL (if applicable)
- Brief attribution
- Date processed
