# Decision Log

> Key architectural, business, and strategic decisions across the portfolio.

---

## Format

Each entry: **Date | Project | Decision | Rationale | Status**

---

## Decisions

### Architecture

| Date | Project | Decision | Rationale | Status |
|---|---|---|---|---|
| 2025 | Before Maps | Next.js 16 + Sanity v5 + Tailwind v4 | Modern stack, ISR for performance, embedded CMS | Active |
| 2025 | Ms Paul Therapies | Same stack as Before Maps | Consistency, shared knowledge | Active |
| 2025 | Hobie | Vite + React (no Next.js) | SPA is sufficient, no SSR needed, PWA focus | Active |
| 2025 | Both Sanity projects | Embedded Studio at `/studio` | No separate CMS domain needed | Active |
| 2025 | Before Maps | richText type for all descriptions | Enable formatting in CMS, better editorial control | Active |
| 2025 | Before Maps | RichTextRenderer component | Single component handles both string and Portable Text | Active |
| 2025 | Hobie | localStorage-first with Supabase sync | Works offline (PWA), cloud backup optional | Active |
| 2025 | Hobie | Wall-clock timers (Date.now()) | Browser throttles setInterval in background tabs | Active |

### Business

| Date | Project | Decision | Rationale | Status |
|---|---|---|---|---|
| 2025 | Before Maps | Application-based (not open booking) | Quality control, right-fit travelers | Active |
| 2025 | Before Maps | Transparent tiered pricing | Builds trust, explains scouting costs | Active |
| 2025 | Before Maps | Small groups (8–12) | Maintain experience quality | Active |
| 2025 | Ms Paul Therapies | Cal.com + Google Forms (no custom backend) | Simple, reliable, no maintenance | Active |
| 2025 | Ms Paul Therapies | Kit for newsletter | Industry standard, good deliverability | Active |

### Content

| Date | Project | Decision | Rationale | Status |
|---|---|---|---|---|
| 2025 | All | Markdown-first content repos | Version controlled, portable, AI-readable | Active |
| 2025 | All | CLAUDE.md + AGENTS.md pattern | Standardized AI context for every repo | Active |
| 2025 | All | docs/lessons/ folder | Hard-learned rules survive context resets | Active |
| 2025 | Portfolio | Uddip-OS master repo | Single source of truth for the ecosystem | Active |
