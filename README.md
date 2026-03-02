<p align="center">
  <img src="openclaw-bible.jpg" alt="The OpenClaw Bible" width="100%">
</p>

# The OpenClaw Bible

> **every openclaw user must read these 10 hidden prompts that mass-produce ultimate $0 stacks that feel ILLEGAL before you get HACKED in 5 minutes while your agent takes over 4 phones, builds a company from scratch & earns $1,000s a week — here's the setup guide Opus 4.6 built after I fed it 20+ articles while mass-purchasing used Pixels from eBay in my underwear**

...is what your timeline sounds like right now.

You've mass-bookmarked 47 threads. Installed 12 skills you've never used. Copied three different SOUL.md templates that contradict each other. Your agent still sounds like a call centre & your Anthropic bill is $800. You have six tabs open and a growing suspicion that everyone on X has a working setup except you.

Here's the thing. You don't have an OpenClaw problem. You have an *information overload* problem.

Every day brings a new "ultimate guide" that's actually a mass-repackaged Reddit post from someone who installed it yesterday. The signal-to-noise ratio is brutal and getting worse. Your bookmarks folder is a graveyard of good intentions you will never revisit. You know this. I know this. We all know this.

**This guidebook is the opposite of that.**

No threads. No engagement bait. No "secret sauce dumps" that are just the docs rewritten in tweet format. One structured walkthrough - 12 chapters, in order, tested on real setups - that takes you from install to autonomous agent without needing to open another tab.

Read it once. Do the steps. Close your bookmarks folder.

> **Want to follow along interactively?** Open this folder in Claude Code. It will walk you through each chapter step-by-step, prompting you to install, configure, and set up as you go. See [CLAUDE.md](CLAUDE.md) for details.

---

## What's New in 2026.3.1

OpenClaw has shipped 13 releases since the last guidebook update (2026.2.17 → 2026.3.1). The highlights:

- **30+ security fixes** — Sandbox escapes, symlink attacks, SSRF, auth bypasses, exec approval hardening. If you're below 2026.2.25, update immediately.
- **External secrets management** — `openclaw secrets` CLI for managing API keys outside config files
- **Nested sub-agents** — Sub-agents can now spawn their own sub-agents, with configurable depth limits
- **ACP thread-bound agents** — Agents can bind to specific conversation threads for persistent context
- **Agent bindings** — `openclaw agents bind/unbind` for declarative agent-to-channel mapping
- **Session cleanup CLI** — `openclaw sessions cleanup` for managing stale sessions and reducing costs
- **MMR memory re-ranking** — Maximal Marginal Relevance for smarter memory retrieval in multi-agent setups
- **Lifecycle status reactions** — Heartbeats now emit status reactions for coordination visibility
- **New providers** — Gemini 3.1, Kilo Gateway (multi-provider routing), Volcano Engine/BytePlus, Moonshot video generation, Kimi web search
- **Android app** — OpenClaw now runs on Android
- **Claude 4.6 adaptive thinking** — Default brain model now uses adaptive reasoning depth
- **OpenAI WebSocket streaming** — Real-time streaming for OpenAI provider connections

---

## Chapters

### Getting Started
1. **[Getting Started](1.%20Getting%20Started.md)** — Hardware, installation, first setup, models, messaging, workspace
2. **[Core Concepts & Architecture](2.%20Core%20Concepts%20%26%20Architecture.md)** — Brains & muscles, heartbeats, cron, memory, mission control
3. **[Security & Hardening](3.%20Security%20%26%20Hardening.md)** — Three rules, isolation, DM pairing, tool lockdown, emergency procedures, external secrets, 2026.3.1 hardening

### Configuration
4. **[Identity & Personality Files](4.%20Identity%20%26%20Personality%20Files.md)** — SOUL.md, PRINCIPLES.md, AGENTS.md, USER.md, MEMORY.md, ideas library
5. **[Use Cases & Workflows](5.%20Use%20Cases%20%26%20Workflows.md)** — Reverse prompting, use cases, ready-to-use prompts
6. **[Life Automation Audit](6.%20Life%20Automation%20Audit.md)** — Not sure what to automate? Full 9-domain life audit prompt

### Capabilities
7. **[Skills System](7.%20Skills%20System.md)** — SKILL.md format, installing & building skills, progressive disclosure
8. **[Tools & Plugins](8.%20Tools%20%26%20Plugins.md)** — Firecrawl, Summarize, camofox-browser, x-research, Obsidian CLI
9. **[Cost Optimization & Model Routing](9.%20Cost%20Optimization%20%26%20Model%20Routing.md)** — Model tiers, ClawRouter, spending limits, $0 stack

### Advanced
10. **[Content Curation & Swipe Files](10.%20Content%20Curation%20%26%20Swipe%20Files.md)** — Content pipeline, tweet analysis, swipe file system, Typefully
11. **[Multi-Agent Coordination](11.%20Multi-Agent%20Coordination.md)** — Topologies, shared context, roundtables, sub-agents, agent bindings, nested sub-agents, ACP threads
12. **[Marketing Automation & Vibe Marketing](12.%20Marketing%20Automation%20%26%20Vibe%20Marketing.md)** — SEO automation, social media management, ad generation, content automation, zero-cost agency-level marketing

### Appendices
- **[CLI Command Reference](Appendix%20A%20-%20CLI%20Command%20Reference.md)** — All `openclaw` CLI commands including secrets, sessions, and agent bindings
- **[Security Templates](Appendix%20B%20-%20Security%20Templates.md)** — Hardened SOUL.md, Docker sandbox, tool policies, file permissions
- **[Mission Control](Appendix%20C%20-%20Mission%20Control.md)** — Full dashboard build prompt
- **[Changelog](CHANGELOG.md)** — Track all additions and updates

---

## Quick Reference

| What | Where |
|------|-------|
| Choose hardware | [Getting Started](1.%20Getting%20Started.md#choose-your-device) |
| Install OpenClaw | [Getting Started](1.%20Getting%20Started.md#install-openclaw) |
| Choose a model | [Getting Started](1.%20Getting%20Started.md#model-provider) |
| Set up morning brief | [Getting Started](1.%20Getting%20Started.md#b-set-up-morning-brief) |
| Mac Mini setup | [Getting Started](1.%20Getting%20Started.md#dedicated-hardware-setup-optional) |
| Security checklist | [Security & Hardening](3.%20Security%20%26%20Hardening.md#security-checklist) |
| Emergency procedures | [Security & Hardening](3.%20Security%20%26%20Hardening.md#emergency-procedures) |
| Configure agent personality | [Identity Files](4.%20Identity%20%26%20Personality%20Files.md#soulmd-personality--voice) |
| Don't know what to automate | [Life Automation Audit](6.%20Life%20Automation%20Audit.md) |
| Reverse prompting | [Use Cases](5.%20Use%20Cases%20%26%20Workflows.md#the-reverse-prompting-mindset) |
| Add skills | [Skills System](7.%20Skills%20System.md#installing-skills) |
| Connect Obsidian vault | [Tools & Plugins](8.%20Tools%20%26%20Plugins.md#obsidian-cli) |
| Reduce costs | [Cost Optimization](9.%20Cost%20Optimization%20%26%20Model%20Routing.md#the-model-hierarchy) |
| Build a content pipeline | [Content Curation](10.%20Content%20Curation%20%26%20Swipe%20Files.md) |
| Automate marketing | [Marketing Automation](12.%20Marketing%20Automation%20%26%20Vibe%20Marketing.md) |

---

## Sources & Credits

This guidebook was compiled from:
- Atlas/jonnym1ller — Agent principles and identity file philosophy
- YJstacked — Claude Skills deep dive, agent swarms article
- Hoeem — Life Automation Audit
- Corey Haines — Marketing skills collection
- Voxyz/Voxyz_ai — Multi-agent system tutorial
- Alex Finn — 210-hour OpenClaw usage lessons
- OpenClaw community — Use cases, tips, and workflows
- Various community contributors on Discord and Twitter/X
