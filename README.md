# 🔬 skill-code-review

> Systematic code review patterns for AI agents.

A **skill** for [StratusOS](https://stratuslabs.io) — the AI operating system for Mac.

---

## What it does

Teaches any agent how to review code like a senior engineer — security vulnerabilities, performance issues, maintainability concerns, and style consistency. Includes structured output formats for GitHub PR comments, severity ratings, and actionable fix suggestions.

## Installation

```bash
# From StratusOS Marketplace (recommended)
# Open StratusOS → Marketplace → Skills → Code Review → Install

# Or manual:
git clone https://github.com/stratuslabs/skill-code-review.git ~/.stratusos/skills/code-review
```

## What's included

```
SKILL.md                — Core review methodology
templates/
  pr-review.md          — GitHub PR review format (severity + findings + suggestions)
  security-audit.md     — Security-focused review checklist
  performance-review.md — Performance bottleneck analysis
  refactor-plan.md      — Refactoring recommendations with effort estimates
```

## Review categories

- **Security** — injection, auth bypass, data exposure, secrets in code
- **Performance** — N+1 queries, memory leaks, unnecessary allocations
- **Correctness** — race conditions, edge cases, error handling
- **Maintainability** — naming, complexity, dead code, missing tests
- **Style** — consistency, formatting, idiomatic patterns

## How skills work

Skills are pure knowledge — no binaries, no APIs. When loaded, the skill's `SKILL.md` and templates are injected into the agent's context. The agent learns the review methodology and applies it to any codebase.

## Requirements

- StratusOS v0.2.0+

---

<p align="center">
  <br>
  Built for <a href="https://stratuslabs.io"><strong>StratusOS</strong></a> — your AI operating system.
  <br>
  <a href="https://github.com/stratuslabs">GitHub</a> · <a href="https://discord.gg/PNJseAMbPn">Discord</a>
  <br>
  <br>
  <sub>Made by <a href="https://github.com/stratuslabs">Stratus Labs</a></sub>
</p>
