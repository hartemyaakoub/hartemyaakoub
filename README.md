<div align="center">

### Yaakoub HARTEM

**Founder & CEO, [TKAWEN](https://tkawen.com)** · Building real-time infrastructure from 🇩🇿 Algeria, for the world.

[![liqaa](https://img.shields.io/badge/LIQAA-Cloud-1d4ed8?style=flat-square)](https://liqaa.io)
[![tkawen](https://img.shields.io/badge/TKAWEN-Group-0a0d18?style=flat-square)](https://tkawen.com)
[![algeriacertify](https://img.shields.io/badge/Algeria_Certify-Live-10b981?style=flat-square)](https://algeriacertify.com)
[![mystoq](https://img.shields.io/badge/MyStoq-Live-7c3aed?style=flat-square)](https://mystoq.com)

[![Email](https://img.shields.io/badge/email-yaakoub.hartem.mhsi%40gmail.com-475569?style=flat-square)](mailto:yaakoub.hartem.mhsi@gmail.com)
[![X](https://img.shields.io/badge/x-%40liqaa__io-0f172a?style=flat-square&logo=x)](https://x.com/liqaa_io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Yaakoub_HARTEM-0a66c2?style=flat-square&logo=linkedin)](https://linkedin.com/in/hartem-yaakoub)

</div>

---

### What I'm shipping

I run **TKAWEN** — a sovereign-tech company building infrastructure for the MENA region and beyond. Our flagship products power production traffic for thousands of users daily.

**LIQAA** is the public-facing piece: a Stripe-grade video conferencing API with WebRTC under the hood, served from a global edge network. WebRTC simulcast, HMAC-signed webhooks, JWT-based per-user tokens, persistent room reuse — production primitives, not a demo.

**Stack:** TypeScript, Next.js 16, Laravel 12, PHP 8.4, Go, Python, LiveKit SFU, MySQL, Redis, nginx, systemd, Docker, GitHub Actions, Vercel, Cloudflare R2.

---

### LIQAA — the open-source ecosystem

This isn't a single repo. It's a **17-repo platform** — every artifact a developer needs, in their language, with their workflow.

#### 🧰 SDKs · meet developers in their language

| Repo | Lang | Package | What it does |
| ---- | ---- | ------- | ------------ |
| 🏆 [`liqaa-js`](https://github.com/hartemyaakoub/liqaa-js) | TypeScript | `@liqaa/js` | Drop-in `<script>` + npm — React, Next.js, Vue, Vanilla examples |
| 🐘 [`liqaa-php`](https://github.com/hartemyaakoub/liqaa-php) | PHP | `liqaa/sdk` | Composer — Laravel + Symfony-friendly |
| 🐍 [`liqaa-python`](https://github.com/hartemyaakoub/liqaa-python) | Python | `liqaa` | PyPI · Flask, Django, FastAPI |
| 🐹 [`liqaa-go`](https://github.com/hartemyaakoub/liqaa-go) | Go | — | `go get` module, idiomatic |

#### 🛠 Tooling · how developers actually use it

| Repo | What it does |
| ---- | ------------ |
| ⌨️ [`liqaa-cli`](https://github.com/hartemyaakoub/liqaa-cli) | `npx @liqaa/cli` — login, rooms, tokens, webhooks, deliveries, status, shell completion |
| 🤖 [`liqaa-mcp`](https://github.com/hartemyaakoub/liqaa-mcp) | **Model Context Protocol** — let Claude / Cursor implement video features by prompt |
| 🧩 [`liqaa-vscode`](https://github.com/hartemyaakoub/liqaa-vscode) | VS Code extension — inline docs, room management, webhook tester (in-editor) |

#### 🚀 Templates · zero-friction starters

| Repo | Stack | Time-to-call |
| ---- | ----- | ------------ |
| ⚡ [`liqaa-template-nextjs`](https://github.com/hartemyaakoub/liqaa-template-nextjs) | Next.js 16 · App Router · RSC · webhook handler | < 3 min |
| ⚛️ [`liqaa-template-react`](https://github.com/hartemyaakoub/liqaa-template-react) | React 19 · Vite · TypeScript | < 3 min |

#### 📜 Specs · single source of truth

| Repo | What it is |
| ---- | ---------- |
| 📜 [`liqaa-openapi`](https://github.com/hartemyaakoub/liqaa-openapi) | OpenAPI 3.1 spec — the **only** description of the API. Every SDK derives from this |
| 🏛️ [`liqaa-architecture`](https://github.com/hartemyaakoub/liqaa-architecture) | Public **Architecture Decision Records** + system diagrams. The "why" behind every choice |

#### 🔭 Operations · radical transparency

| Repo | What it is |
| ---- | ---------- |
| 🟢 [`liqaa-status`](https://github.com/hartemyaakoub/liqaa-status) | Public uptime probes — every 5 min via GitHub Actions, history is git log |
| 📊 [`liqaa-benchmarks`](https://github.com/hartemyaakoub/liqaa-benchmarks) | Reproducible latency + cost benchmarks · LIQAA vs Daily, Twilio, LiveKit Cloud, Whereby |

#### 📣 Community

| Repo | What it is |
| ---- | ---------- |
| ✨ [`awesome-liqaa`](https://github.com/hartemyaakoub/awesome-liqaa) | Curated list — SDKs, integrations, community resources |
| 📰 [`liqaa-changelog`](https://github.com/hartemyaakoub/liqaa-changelog) | Public changelog (Keep-a-Changelog · semantic versioning) |
| 🗺️ [`liqaa-roadmap`](https://github.com/hartemyaakoub/liqaa-roadmap) | What we're shipping — Q2/Q3/Q4 2026 + 2027 horizon |

---

### Engineering principles

I optimise for things that compound. The repos above aren't a marketing checklist — each one closes a specific developer-trust loop.

- **`pk_live_` / `sk_live_` separation** ([ADR-002](https://github.com/hartemyaakoub/liqaa-architecture/blob/main/adrs/002-stripe-pattern-pk-sk-key-separation.md)) — Stripe got this right in 2011, no point reinventing it.
- **JWT token exchange** ([ADR-003](https://github.com/hartemyaakoub/liqaa-architecture/blob/main/adrs/003-jwt-token-exchange-vs-long-lived-keys.md)) — never ship a long-lived secret to a browser.
- **HMAC-signed webhooks with replay protection** ([ADR-004](https://github.com/hartemyaakoub/liqaa-architecture/blob/main/adrs/004-hmac-sha256-webhooks-with-replay-protection.md)) — the t=…,v1=… pattern.
- **No PII in storage paths** ([ADR-005](https://github.com/hartemyaakoub/liqaa-architecture/blob/main/adrs/005-no-pii-in-recording-paths.md)) — opaque IDs, not customer emails.
- **OpenAPI as single source of truth** ([ADR-008](https://github.com/hartemyaakoub/liqaa-architecture/blob/main/adrs/008-openapi-as-single-source-of-truth.md)) — every SDK derives from one spec.
- **Public status page powered by GitHub Actions** ([ADR-009](https://github.com/hartemyaakoub/liqaa-architecture/blob/main/adrs/009-public-status-page-via-github-actions.md)) — incident history is git log.

The full ADR set is in [`liqaa-architecture`](https://github.com/hartemyaakoub/liqaa-architecture).

---

### Reach out

- **Partners / sales:** [partners@tkawen.com](mailto:partners@tkawen.com)
- **Security:** [security@liqaa.io](mailto:security@liqaa.io) · [security.txt](https://liqaa.io/.well-known/security.txt)
- **Personal:** [yaakoub.hartem.mhsi@gmail.com](mailto:yaakoub.hartem.mhsi@gmail.com)

---

<div align="center">

[![GitHub stats](https://github-readme-stats.vercel.app/api?username=hartemyaakoub&theme=transparent&hide_border=true&include_all_commits=true&count_private=false&show_icons=true)](https://github.com/hartemyaakoub)
[![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=hartemyaakoub&theme=transparent&hide_border=true&layout=compact)](https://github.com/hartemyaakoub)

> Built in 🇩🇿 Algeria, for the world.

</div>
