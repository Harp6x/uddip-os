# Portfolio Dependency Map

> How all 5 projects connect — shared infrastructure, content flows, and cross-project relationships.

---

## Shared Infrastructure

```
┌──────────────────────────────────────────────────────────┐
│                      GITHUB (Harp6x)                     │
│  beforemaps · hobie · misspaultherapies                  │
│  uddip-content · aishani-content · uddip-os              │
└──────────────────────────────────────────────────────────┘
                            │
                            ▼
┌──────────────────────────────────────────────────────────┐
│                        VERCEL                            │
│  Before Maps · Hobie · Ms Paul Therapies                 │
│  (auto-deploy from GitHub main branch)                   │
└──────────────────────────────────────────────────────────┘
```

---

## CMS Infrastructure

```
SANITY.IO
├── Project: c4zc1cd4 (Before Maps)
│   ├── Dataset: production
│   ├── 15 document types
│   └── Studio at: /studio
│
└── Project: k0r3y2my (Ms Paul Therapies)
    ├── Dataset: production
    ├── 12 document types
    └── Studio at: /studio
```

**Pattern:** Both Sanity projects use the same architecture — embedded studio, GROQ queries, ISR with `revalidate: 60`.

---

## Content Flow

```
Uddip Content ──┬──→ HARP6X (social media, blog)
                ├──→ ThereGoesUddip (social, YouTube)
                └──→ Before Maps Sanity CMS → beforemaps.com

Aishani Content ───→ Ms Paul Therapies Sanity CMS → mspaultherapies.in
                ───→ Instagram, YouTube (direct)
```

---

## Shared Technology

| Technology | Before Maps | Hobie | Ms Paul Therapies |
|---|:---:|:---:|:---:|
| React 19 | ✓ | ✓ | ✓ |
| TypeScript | ✓ | ✓ | ✓ |
| Tailwind CSS v4 | ✓ | ✓ | ✓ |
| Lucide Icons | ✓ | ✓ | ✓ |
| Next.js 16 | ✓ | — | ✓ |
| Sanity v5 | ✓ | — | ✓ |
| @portabletext/react | ✓ | — | ✓ |
| Vercel Analytics | ✓ | ✓ | ✓ |
| Vitest | ✓ | — | ✓ |
| Supabase | — | ✓ | — |
| PWA | — | ✓ | — |

---

## Cross-Project Relationships

```
Before Maps ←──content──→ Uddip Content (before-maps/ folder)
    │
    └──shared founder──→ Ms Paul Therapies (Uddip manages both)

Ms Paul Therapies ←──content──→ Aishani Content
    │
    └──same architecture as──→ Before Maps (Next.js + Sanity + Tailwind)

Hobie ←──no direct dependency──→ (standalone app)
    │
    └──same founder/deployer──→ All projects

Uddip Content ←──strategy docs──→ Aishani Content
    │                              (shared _os/ patterns)
    └──powers 3 brands──→ HARP6X, TGU, Before Maps
```

---

## Shared Domains & DNS

| Domain | Project | Registrar | Notes |
|---|---|---|---|
| beforemaps.com | Before Maps | — | Primary domain |
| mspaultherapies.in | Ms Paul Therapies | — | Primary domain |
| mspaultherapies.com | Ms Paul Therapies | — | Redirects → .in |
| hobie-deploy.vercel.app | Hobie | Vercel | Vercel subdomain |

---

## Shared Design Patterns

1. **CMS-driven pages with hardcoded fallbacks** — Both Before Maps and Ms Paul Therapies fetch from Sanity first, fall back to static content when empty
2. **Lesson docs** — All code repos have `docs/lessons/` with hard-learned rules
3. **CLAUDE.md + AGENTS.md pattern** — Standardized AI context files at repo root
4. **ISR with revalidate: 60** — Shared caching strategy across Next.js projects
5. **Component architecture** — `src/components/sections/` for page sections, `src/components/ui/` for shared UI

---

## Shared Workflows

| Workflow | How It Works |
|---|---|
| **Deploy** | Push to `main` → Vercel auto-deploys |
| **Content publish** | Write markdown → push to content repo → seed into Sanity CMS |
| **CI** | GitHub Actions (Before Maps has `ci.yml`; Ms Paul Therapies has similar) |
| **Testing** | `npm test` (Vitest) → `npm run typecheck` → `npm run build` |
| **Docs** | Update `CLAUDE.md` + `docs/AGENTS.md` after architectural changes |
