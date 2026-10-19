# Following the AI Audit Trail

**BSides NYC 2026 · October 17, 2026**

Darwin Salazar (@darwnsm) · [Monad](https://monad.com) · The Cybersecurity Pulse

A map of what AI agents log, where to find it, and what it misses.

📄 **[Slides (PDF)](./Following_the_AI_Audit_Trail_BSides_NYC_2026.pdf)**

## What the talk covers

- **AI audit logs in 2026 are where cloud audit logs were in 2018.** Field names change between versions, products merge, and security teams are still working out what gets logged.
- **Four questions, four kinds of evidence:** platform audit records, runtime events (usually OpenTelemetry), transcripts and content capture, and evidence from outside the agent.
- **Who gives you what:** Claude Code, Claude Cowork, OpenAI Codex, Cursor, GitHub Copilot, the Anthropic Activity Feed and compliance transcripts, OpenAI API Platform audit logs, and Gemini for Workspace.
- **Cloud audit logs then, agent telemetry now:** Azure Activity Log and AWS CloudTrail field by field against Claude Code telemetry.
- **Live demo:** three Claude Code runs (manual approval, manual rejection, auto mode) and what each one leaves in the `tool_decision` and `tool_result` events.
- **Where to start**, plus starting hunts for sensitive paths, accepted decisions with no result, automatic approvals against policy, and silent clients.

The appendix has the full source comparisons, Claude Code telemetry settings, and the setup to reproduce the demo on your own laptop.

## Go deeper

- *A Security Field Guide to AI Audit Trails* (Monad, October 2026), the book this talk is based on
- [Claude Code monitoring docs](https://code.claude.com/docs/en/monitoring-usage)
- [monad-inc/community-transformations](https://github.com/monad-inc/community-transformations), the open-source split-and-flatten transform from slide 8
- Detection engineering for Claude Code, [part 1](https://monad.com/blog/detection-engineering-for-claude-code-part-1) and [part 2](https://monad.com/blog/detection-engineering-for-claude-code-part-2) (Monad blog, March 2026)
- [AI Agent Artifact Catalog](https://depalmar.github.io/ai-dfir-toolkit)
- [OWASP Top 10 for Agentic Applications](https://genai.owasp.org)
- [MITRE ATLAS](https://atlas.mitre.org)
