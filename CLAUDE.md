@AGENTS.md

## Claude Code notes
- AGENTS.md above is shared with Codex. Put shared guidance there; this section is for Claude-only behavior.
- Start every Build session in plan mode. Give it the change's intent.md and spec.md and ask for a plan that names the files that change, the order of work and the tests that prove it. Commit the accepted plan as plan.md before writing code.
- Hooks (`.claude/settings.json`) and the verifier subagent (`.claude/agents/`) arrive in Phase 2.
