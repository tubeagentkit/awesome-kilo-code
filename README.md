# Awesome Kilo Code

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated directory of skills, MCP servers, agents, and community tools for [Kilo Code](https://github.com/Kilo-Org/kilocode) — the open-source agentic coding platform (27k+ stars, actively developed).

Kilo Code ships with a large official marketplace of skills, MCP servers, and agents, but it's spread across folders and hard to browse from outside the editor. This list pulls the useful parts together in one place, and adds the real community tools built around it — honestly labeled, no padding.

---

## ⭐ Featured Skill

> **youtube-transcript-skills** — Fetch YouTube video transcripts, search videos and channels, browse channel uploads, and extract playlists. No Google API key, no yt-dlp, no headless browser.
>
> ```bash
> npx skills add tubeagentkit/youtube-transcript-skills
> ```
>
> Try it: *"Summarize this video and tell me what channel it's from: <a YouTube URL>"* — Kilo Code fetches the transcript and channel info in one call. Powered by the free tier of [getyoutubetranscript.com](https://getyoutubetranscript.com) (100 credits, no card required). Also available as a remote MCP server if you'd rather connect it that way — see [tubeagentkit/youtube-mcp](https://github.com/tubeagentkit/youtube-mcp).

---

## Quick Start

1. **Install Kilo Code** — [VS Code extension](https://marketplace.visualstudio.com/items?itemName=kilocode.Kilo-Code) or the [kilocode CLI](https://github.com/Kilo-Org/kilocode). Free tier included, no account required to start.
2. **Browse the official marketplace** from inside the editor (`Kilo Code: Browse Marketplace`) — this is where the built-in skills/MCP servers/agents below live.
3. **Try the featured skill above**, then explore what else is here.

---

## Kilo's Own Marketplace (official, built-in)

The [`Kilo-Org/kilo-marketplace`](https://github.com/Kilo-Org/kilo-marketplace) repo is Kilo's real, first-party catalog — this list doesn't duplicate it, just points at real numbers so you know what's already there before looking elsewhere:

| Resource | Count (verified 2026-09-27) | What it is |
|---|---|---|
| [Skills](https://github.com/Kilo-Org/kilo-marketplace/tree/main/skills) | 180+ | `SKILL.md`-format packages using the open [Agent Skills spec](https://agentskills.io/) — data engineering, cloud platforms (AWS/Azure/GCP), databases, frontend, and more |
| [MCP Servers](https://github.com/Kilo-Org/kilo-marketplace/tree/main/mcps) | 130+ | Pre-configured MCP connections — GitHub, Slack, Stripe, Notion, Postgres, Playwright, and many more |
| [Agents](https://github.com/Kilo-Org/kilo-marketplace/tree/main/agents) | 8 official (architect, code-reviewer, code-simplifier, code-skeptic, test-engineer, data, docs-specialist, frontend-specialist) | Kilo's current orchestration primitive — replaced "Modes" (Kilo 5.x, now legacy) |
| [Plugins](https://github.com/Kilo-Org/kilo-marketplace/tree/main/plugins) | 2 (git, opencode-models-discovery) | Runtime extensions: hooks, custom tools, auth/model providers |

**Note on Modes vs. Agents:** Kilo is actively migrating from "Modes" (a legacy concept from Kilo 5.x) to "Agents." If you find older content referencing Modes, it may be outdated for current Kilo versions.

---

## Community Tools

Real, independently-built tools that work with Kilo Code (verified active as of 2026-09-27, not abandoned):

- [**codexmate**](https://github.com/SakuraByteCore/codexmate) — One dashboard for all your local AI coding agents: switch providers, manage sessions, and orchestrate tasks across Codex, Claude Code, Gemini CLI, KiloCode, OpenClaw and more. Local-first, zero cloud.
- [**Superlearn**](https://github.com/raiyanyahya/Superlearn) — Learn anything, deeply, from inside Claude Code, Codex, or Kilo Code.
- [**agentMemory**](https://github.com/webzler/agentMemory) — Persistent memory layer to reduce AI hallucinations; zero-config, works with Cline, RooCode, and KiloCode.
- [**kilocode-agents**](https://github.com/galpt/kilocode-agents) — Prompt and agent presets for stronger multi-agent workflows in Kilo Code.
- [**KiloCode-CustomModes-DualDesign**](https://github.com/Nikolay-Shirokov/KiloCode-CustomModes-DualDesign) — A dual-role custom mode setup for structured design + implementation workflows.
- [**kilocode-rules**](https://github.com/shanefully-done/kilocode-rules) — A ruleset for keeping Kilo Code's output consistent across a project.
- [**oc-go-usage-display**](https://github.com/christophkroeppl/oc-go-usage-display) — Live OpenCode Go plan usage (5h / 7d / 30d windows) as a Kilo Code sidebar block and statusline, plus a `go_usage` tool your agent can call; installs as a native Kilo plugin (`kilo.json` + `tui.json`) and reads Kilo's own auth store, so there is nothing to paste.

*This section is honestly small — Kilo Code's third-party ecosystem is still young relative to its 27k-star install base. If you've built something real for Kilo Code, open a PR.*

---

## MCP Servers Beyond the Official Marketplace

Kilo Code connects to any standard MCP server, not just the ones pre-configured in its marketplace. A few real, actively-maintained ones worth knowing about beyond what's already listed above:

- [**tubeagentkit/youtube-mcp**](https://github.com/tubeagentkit/youtube-mcp) — YouTube transcripts, video/channel search, channel browsing, playlist extraction. Free tier, OAuth 2.1 or API key.
- [**context7**](https://github.com/upstash/context7) — Up-to-date library documentation, already in Kilo's own marketplace but worth knowing works everywhere.
- [**playwright-mcp**](https://github.com/microsoft/playwright-mcp) — Official Microsoft browser automation MCP server, also in Kilo's marketplace.

For a broader directory of general-purpose MCP servers (not Kilo-specific), see [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers).

---

## More from tubeagentkit

YouTube tools for AI agents, built on the [GetYouTubeTranscript API](https://getyoutubetranscript.com):

- [youtube-transcript-api](https://github.com/tubeagentkit/youtube-transcript-api): YouTube Transcript API docs, endpoint reference, OpenAPI spec and examples in curl, Python, JavaScript, Go and PHP
- [youtube-transcript-api-python](https://github.com/tubeagentkit/youtube-transcript-api-python): YouTube Transcript API SDK for Python
- [youtube-transcript-api-node](https://github.com/tubeagentkit/youtube-transcript-api-node): YouTube Transcript API SDK for Node.js / TypeScript
- [youtube-mcp](https://github.com/tubeagentkit/youtube-mcp): Remote YouTube MCP server for Claude, ChatGPT, Cursor and VS Code
- [youtube-transcript-skills](https://github.com/tubeagentkit/youtube-transcript-skills): YouTube transcript Agent Skill for Claude Code, Cursor, Codex and OpenClaw
- [youtube-transcript-cursor-plugin](https://github.com/tubeagentkit/youtube-transcript-cursor-plugin): YouTube Transcript Cursor plugin bundling the MCP server, skills, commands and a research agent
- [n8n-nodes-getyoutubetranscript](https://github.com/tubeagentkit/n8n-nodes-getyoutubetranscript): YouTube transcript n8n community node, also usable as an AI Agent tool

## Contributing

Found a real, actively-maintained tool for Kilo Code that isn't here? Open a PR:

- One entry per PR, in the right section.
- Link to a real, maintained repo (check it has commits in the last few months).
- One sentence: what it does, in plain language.
- No self-promotion for products with no real Kilo Code integration — this list stays honest about what's actually built for Kilo Code vs. generically compatible.

## License

MIT — see [LICENSE](./LICENSE).
