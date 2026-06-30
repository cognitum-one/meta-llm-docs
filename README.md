# Cognitum MetaHarness-as-a-Service — public docs

Public landing page and high-level documentation for **Cognitum MetaHarness-as-a-Service (MaaS)** — a
multi-tenant, tiered, metered, budget-governed, dual-protocol (OpenAI + Anthropic) Completions API,
plus autonomous Darwin-Loop agent pods with human approval gates, on Google Cloud.

**Live site:** https://cognitum-one.github.io/meta-llm-docs/

## Honest framing

Cognitum MaaS is a **governance / cost / safety / multi-tenancy platform on commodity models at a
measured Pareto cost-corner — not a frontier model**. Orchestration here is a **cost lever, not an
accuracy lever**. See [`status.html`](status.html) for the honest built-vs-roadmap ledger.

## What's here

| Page | Content |
|------|---------|
| `index.html` | Landing — what MaaS is, the honest framing, the three dials, the value prop |
| `capabilities.html` | Conceptual capabilities overview (tier / host / approval gate, pods, metering + budget) |
| `architecture.html` | High-level layered request pipeline + pod substrate (sanitized) |
| `status.html` | Honest live / built / design / open status ledger |
| `SECURITY.md` + `.well-known/security.txt` | Security policy + contact (RFC 9116) |

## This is a static site

Plain HTML + a single self-hosted stylesheet. **No build step, no JavaScript, no analytics, no
trackers, no external CDNs, no cookies.** It can be opened directly in a browser.

## Privacy & secrets

This repository contains **no** application code, API keys, secrets, or private internals. The
product's API and source code are private and auth-gated. The public API endpoint name is mentioned
because it is already public and authentication-gated.

## Related, but distinct

This is the **platform** documentation. The MetaHarness Studio and the AgentBBS arena are separate
surfaces built on top of the platform and are documented elsewhere.
