# 魏宇霆 David Wei

Founder of **BTF Culture & Creative (傲嬌文創)** and **Alljoint (傲嬌軟體)**, Taipei.

I run a one-person software company. Over the past year I built an AI-agent
development workflow (Claude Code + Codex, with Claude planning/reviewing and
Codex implementing) and used it to ship and operate several production SaaS
products for Taiwanese SMBs, plus dozens of internal tools that automate most
of my company's day-to-day operations.

Most of my product code lives in private repos because it runs real businesses
with real customer data. This page is the public index.

## Live products

| Product | What it is | Stack |
|---|---|---|
| [work.btf.tw](https://work.btf.tw) | Shift scheduling + HR/payroll SaaS for retail and restaurant stores. Multi-store, 4 roles, claim-a-shift scheduling, clock-in, payroll with Taiwan labor/health insurance deductions, leave, expense claims, bonuses, daily revenue analytics, LINE push notifications. Used by real stores daily. | Next.js 15, TypeScript, Supabase (Postgres + RLS), Vercel |
| [quotation.alljoint.tw](https://quotation.alljoint.tw) | Quotation system with shareable per-quote links, PDF export and email delivery. | Vanilla JS, Supabase, Vercel |
| [ins.alljoint.tw](https://ins.alljoint.tw) | Mobile quiz app for Taiwan insurance-agent certification exams. | Single static HTML, Supabase (Google login + RLS) |
| [alljoint.tw](https://alljoint.tw) | Company site. | Next.js |

## In progress

- **AI stock screener (TW + US)**: post-market quant and fundamental screening, with Claude-generated plain-Chinese rationale. Multi-tenant.
- **Bonded-warehouse cigar WMS**: batch/vintage tracking, customs bonded ledger export, per-country export compliance checks.
- **Rotary club event registration SaaS**: multi-tenant, row-level isolation per club.
- **Hotel management system** prototype.

## How I work

- Claude plans, Codex implements, both review each other's output. I read every diff.
- Security first: RLS with `WITH CHECK` on every update policy, `SECURITY DEFINER` RPCs for anonymous access, rate limits keyed by IP, no secrets in code. I keep a reusable RLS audit probe that runs as a PR gate.
- Every change is verified on a real environment (DB sandbox transactions, API smoke tests, Playwright screenshots), not just unit tests.

## Earlier

- **Lost & Found Lady (失物小姐)**: LoRa/Sigfox tracker tags for everyday items. Shut down after Apple AirTag launched.
- Early founding member of **Hackathon Taiwan**; mentored open-source and incubator teams.
- First business, in high school: automation bots for an online game, sold through forum word of mouth with a built-in referral feature (friend shares it, first month free).

## Contact

david@alljoint.tw
