# AI Handoff — 15-Minute Onboarding

> You are a new AI model. This document gives you full context on the Uddip ecosystem in under 15 minutes.

---

## Read Order

1. **This file** (5 min) — ecosystem overview, priorities, rules
2. **`MASTER_CONTEXT.md`** (3 min) — who, what, infrastructure
3. **`DEPENDENCY_MAP.md`** (3 min) — how projects connect
4. **Project-specific `CLAUDE.md`** (4 min) — deep context for whichever project you're working on

---

## The Ecosystem in 60 Seconds

Uddip runs 5 projects from India:

- **Before Maps** — travel company (Next.js + Sanity). The biggest, most active codebase.
- **Hobie** — hobby tracker app (Vite + React + Supabase). Smaller, self-contained.
- **Ms Paul Therapies** — therapy website for partner Aishani (Next.js + Sanity). Similar architecture to Before Maps.
- **Uddip Content** — markdown content library (2,100+ files). Powers 3 brands.
- **Aishani Content** — markdown content library (700+ files). Powers Ms Paul Therapies.

All code repos are on GitHub under `Harp6x`. All web apps deploy to Vercel.

---

## Current Priorities (as of June 2025)

1. **Before Maps** — Content seeding, Sanity Studio UX, journey scouting, digital products
2. **Ms Paul Therapies** — Maintenance mode, content updates via Aishani Content
3. **Hobie** — Feature development as time allows
4. **Content repos** — Continuous growth, support publishing workflows

---

## Technical Patterns Across Projects

| Pattern | Before Maps | Ms Paul Therapies | Hobie |
|---|---|---|---|
| **Framework** | Next.js 16 (App Router) | Next.js 16 (App Router) | Vite 8 + React Router 7 |
| **CMS** | Sanity v5 | Sanity v5 | None |
| **Styling** | Tailwind v4 + shadcn/ui | Tailwind v4 | Tailwind v4 |
| **Auth** | None | None | Supabase |
| **Data** | Sanity-first, hardcoded fallback | Sanity-first, static file fallback | localStorage + Supabase |
| **Testing** | Vitest | Vitest | None |
| **Deploy** | Vercel | Vercel | Vercel |

---

## Universal Rules (Apply to ALL Projects)

1. **Never remove features** without explicit founder request
2. **Never break existing pages** — always verify: tsc, test, build, visual check
3. **Read `docs/lessons/`** before every session (each code repo has one)
4. **Don't guess** — use tools to discover. Read files before editing.
5. **Sanity write tokens** may be read-only. Check before running mutations.
6. **Font "Inter":** The style is `"Semi Bold"` (with space), not `"SemiBold"`

---

## Known Issues & Tech Debt

### Before Maps
- Sanity richText migration pending (string → Portable Text blocks). Script exists at `scripts/migrate-richtext.mjs`, needs write token.
- `journey-detail.tsx` (920 LOC) and `journeys-list.tsx` (685 LOC) need splitting
- `mock-data.ts` (1502 LOC) is not imported anywhere — candidate for removal
- Hero slideshow images are hardcoded in `src/components/sections/hero.tsx`
- Products page disabled via `enableProductsPage: false` in Sanity globalSettings

### Hobie
- Pre-existing TS errors from unused Radix UI imports in `ui/` components
- No test suite

### Ms Paul Therapies
- Homepage content mostly hardcoded (pain points, how-it-works, trust badges)
- `src/content/blog.ts` is 40KB with 60+ posts as static fallback

---

## Content Repos — How They Connect

```
Uddip Content (2,100+ files)
├── harp6x/        → HARP6X brand (social, blog, products)
├── theregoesuddip/ → TGU brand (travel, personal essays)
├── before-maps/   → Before Maps brand (journey content, field notes)
└── _os/           → Operating system, strategy, calendars

Aishani Content (700+ files)
├── content/       → Blog, reels, carousels for Ms Paul Therapies
├── digital-products/ → Workbooks, guides
└── mspaultherapies/  → Website-specific content
```

Content flows: **Content Repo → Sanity CMS → Website** (or directly to social media)

---

## How to Work on a Specific Project

1. Read the project's `CLAUDE.md` (root of repo)
2. Read `docs/lessons/` if it exists
3. Check `docs/AGENTS.md` for detailed architecture
4. Run the project's verify commands before and after changes
5. Never push without: `tsc --noEmit` clean, tests passing, build succeeding
