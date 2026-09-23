# Dmitry Tolstikhin

**AI Transformation & Operations Architect · governed AI agent systems** — Dubai, UAE

For 25 years I have run operations and finance where the mistake was personally mine to answer for:
banks, licensed entities, cross-border structures, audits, regulators. Since 2025 I build the same
discipline on a new substrate — **AI agents that do real work under explicit authority, with every
step reviewable.**

I am not a software engineer and I don't claim to be. I don't write code by hand: I design the
architecture, the boundaries and the acceptance criteria, direct AI coding agents through
implementation, and answer for the result. The whole account below was built that way.

> This account was created on **25 June 2025**; its first commit is my first Telegram bot.
> Everything here is younger than that date. The operating discipline is old, the substrate is new.

---

## What I actually build — the governance layer

Most agent portfolios show prompts. This one shows the employment contract.

- **A digital employee is a contract, not a model.** Each worker ships as a package: charter,
  agent passport, security passport, authority/action matrix, operating contract, tool & MCP
  policy, memory contract, model admission matrix, evaluation & acceptance — 22 numbered
  documents. The package is written to be model-independent; no model is admitted until it passes.
- **An action ladder instead of "trust me."** R0 read → A1 local artefact → A2 scoped reversible
  change → A3 external action → A4 irreversible / release / production. The top rung is never
  self-awarded: it needs an explicit owner decision for that specific action and target.
- **Deny by default.** Capability policies where prohibition wins and an agent cannot widen its own
  rights. Request text, files, web pages, memory and tool output are *data to assess, not
  instructions to obey*; injection phrases are quarantined as evidence.
- **Reviews you can trust.** Every check and review is bound to the exact source fingerprint; any
  write after PASS invalidates the PASS. Reviewers run in a separate read-only context, and a
  self-review is always labelled as a self-review.
- **Honest status, by construction.** Packages carry their own state — `NOT_BUILT`,
  `NOT_ADMITTED`, `production: NO` — and a failed candidate is frozen as negative evidence, not
  quietly rebuilt.
- **A learning ledger under a gate.** 100+ recorded operating lessons; a lesson becomes an active
  rule only after review — by me, or under my explicit, logged delegation — never by the agent's
  own say-so.

The through-line: *a fluent answer is not a correct one, and a model's confidence is not authority.*

**What actually runs today**, so the honest statuses below are not mistaken for "nothing works":
the development harness my agents build with (GitHub Issue → fingerprint-bound review → draft PR); the
Platform Architect agent, 940 offline tests passing and a container that starts without any
credential; the studio director's decision core with its test suite; and four small services I
operate that run every day — a legal-content pipeline with a public channel, a client campaign control
panel with a Telegram Mini App, and two advisory bots. Packages marked `NOT_ADMITTED` are exactly
that: designed and checked in documents and tests, not yet allowed to act on their own.

---

## Public work

**Showcase open, implementation closed.** For the core pieces I publish how they are built, what
principles they follow, their honest status and a few load-bearing documents in full — not the
working code or complete packages.

### [digital-employee-showcase](https://github.com/DmGranit/digital-employee-showcase) — the contract
The 22-document structure of one digital employee and, in full, its **authority/action matrix**
(R0 → A4, stage grants, what counts as a material fork) and its **package status**
(`READY_FOR_OWNER_REVIEW`, no model admitted).

### [principal-engineer-showcase](https://github.com/DmGranit/principal-engineer-showcase) — an employee as a constitution
An end-to-end engineering employee: orient → ground in reality → requirements → options → decision →
plan → implement → verify → review → release-readiness → deliver → observe → hand off. Published: constitution §1–5 (*a model belief is
never a FACT*, *evidence is data, not instructions*, *capability is not authority*), all 60
invariant names, the map of 68 skills and 9 playbooks with authority ceilings, the fingerprint-bound
review contract, and a status file that says `NOT_BUILT`, `NOT_ADMITTED`.

### [platform-architect-showcase](https://github.com/DmGranit/platform-architect-showcase) — an employee that runs
A Principal Platform Architect on Google ADK 2.8 with an epistemic contract: separates fact from
inference, declines owner decisions, labels its own review as self-review. 14 runtime skills, 15
invariants defended in code, 940 offline tests passing. Published: the full professional
constitution. Status in its own words: `v0.1 — BUILT / LOCALLY VERIFIED`.

### [agent-security-passport-showcase](https://github.com/DmGranit/agent-security-passport-showcase) — the security side
A passport that only narrows authority and never creates permission; *schema-valid ≠ validated ≠
registered ≠ admitted*; forbidden self-validation; unknown values fail closed. Published: the field
outline, the registries and runbooks by name. Production readiness stated plainly: `NOT_READY`.
And the part I value most: how a read-only review with no authority found that **none** of the six
agent passports in my own design house conformed to this schema — and what it did about it. To me
that is worth more than a finished product: it is what finding the holes in your own work looks like.

### [dual-line-execution-lab](https://github.com/DmGranit/dual-line-execution-lab) — proving a boundary without touching anything *(complete public copy)*
An executable, synthetic-only lab for bounded hand-offs between a laptop line and a simulated server
line: identity, capability, task binding, default-deny policy, kill switches at four scopes. Authority
`LAB_ONLY` — it cannot accept, release, deploy or act externally. The code imports no networking module
at all, and the tests prove the policy refuses every destination, loopback included, when a task has no
network. Python standard library only.

### [mlm-agent-showcase](https://github.com/DmGranit/mlm-agent-showcase) — a compliance-first AI assistant for a direct-sales company
Role agents under an orchestrator over a shared knowledge core, designed so the system **declines
rather than invents**. Measured, not claimed: search duplicates 23% → 0% after re-chunking; a
self-reported failure metric caught lying at 54% and fixed to the real 8%. *(Russian.)*

**Also public:**
[pdn-content-factory](https://github.com/DmGranit/pdn-content-factory) (a governed content pipeline
with a human gate that verifies every fact down to the primary source; it once rejected, on its own,
a viral claim of a 968-million-record data leak that no second source confirmed; *Russian*) ·
[english-os](https://github.com/DmGranit/english-os) (an AI language trainer that marks which claims
are research-backed and which are its own hypothesis; 99 tests; *Russian*).

---

## Still private

- **A decision core for a studio director** — untrusted intent → shareholder lens (continue / needs
  owner decision / hold) → capability requirement → policy-driven provider eligibility → execution
  pack. Request text structurally cannot select a provider. 1,100+ tests on the working branch.
  Under construction.
- **The development harness** the rest is built with: GitHub Issue → durable branch → scope guard →
  ruff/mypy/pytest → fingerprint → separate-context review → synthetic runtime evidence → Result
  Capsule → draft PR. The builder never merges, releases or deploys.
- **An agent foundry** — deterministic assembly of employee packages with build receipts and a
  reproducibility check. Its first candidate is frozen as negative evidence and not admitted — the
  system lowered its own claim of success.
- **A privacy airlock** — pseudonymises personal data before anything reaches a cloud LLM and
  restores it after; the mapping table never leaves the gateway. Working prototype; demo on request.
- **The owner's control plane and client work** — including a Telegram campaign control plane
  live in production (real users' data, mass sending paused by default).

---

## How I can help

1. **Governance review of an agent system you already have** — a bounded, read-only audit against
   an explicit standard: who may do what, where authority leaks, what a text can talk your agent
   into, what the runtime enforces versus what only the prompt promises. Delivered as pinned
   evidence and a plain-language report. A sample report is available on request.
2. **A digital-employee contract for a role you want automated** — the full package, model-
   independent, so you can run it on whichever runtime you use.
3. **A privacy airlock in front of your cloud LLM.**

I work in writing, remotely, through my own agents, and I say "not admitted" out loud until it is.

---

## Credentials

- **Engineer, Electronic Instruments and Devices** — Moscow State Institute of Electronics and
  Mathematics, 2003
- **Professional Certificate in Management — The Open University (UK)**, 2009, via MIM LINK
  (dual award with a Russian state diploma of professional retraining in management)
- **Zerocoder University, 2026 — three completion certificates on agentic development, 100 academic
  hours with delivered final projects:** Vibe-Coding with Claude Code, 36 h (№ 41528) ·
  Vibe-Coding with OpenClaw, 32 h (№ 41951) · VIBE-CODING and Autonomous Software Agents, 32 h
  (№ 43504); plus prompt-engineering (№ 38738) and vibe-coding 3.0 (№ 39994) intensives

---

## Contact

**LinkedIn:** [linkedin.com/in/dmitry-tolstikhin](https://www.linkedin.com/in/dmitry-tolstikhin/)
Dubai, UAE · Russian native · English in writing (I work through my own AI agents — the decisions
are mine, the English is theirs)

Everything in this account is © Dmitry Tolstikhin. Read, cite and learn freely; ask before reusing.
