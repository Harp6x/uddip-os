# Before Maps — Project Summary

**Repo:** `Harp6x/beforemaps` | **Local:** `~/CascadeProjects/beforemaps`
**Live:** beforemaps.com | **Sanity:** c4zc1cd4

---

## Mission
Exploration-led travel company discovering meaningful experiences across India — iconic, emerging, and overlooked places experienced through a different lens.

## Audience
Independent travelers (25–40) who want curated, personally-scouted journeys. Not package tourists.

## Business Model
- Application-based group journeys (8–12 people, transparent tiered pricing)
- Digital travel products (guides, toolkits on Gumroad)
- Retreats (mental health, slow living)
- Custom journeys (bespoke trip design)

## Technology
Next.js 16.2.9 (App Router) · TypeScript · React 19 · Sanity v5 (15 document types) · Tailwind CSS v4 · shadcn/ui · Vercel

## Roadmap
1. Complete Sanity richText data migration
2. Seed all CMS content (journeys, field notes, blog posts, KPIs)
3. Launch first 2–3 journeys
4. Enable products page
5. Pilot first retreat

## Dependencies
- **Uddip Content** — `before-maps/` folder supplies journey content, scouting reports, field notes
- **Sanity CMS** — All editorial content managed via embedded Studio
- **Vercel** — Auto-deploy from GitHub

## Relationship to Other Projects
- Shares Next.js + Sanity + Tailwind architecture with Ms Paul Therapies
- Content sourced from Uddip Content repo (before-maps/ folder)
- No direct dependency on Hobie or Aishani Content

## Documentation
| Doc | Purpose |
|---|---|
| `CLAUDE.md` | AI standalone context |
| `docs/AGENTS.md` | Full AI context with schema map |
| `docs/ARCHITECTURE.md` | System design, data flow |
| `docs/CONTENT-STRATEGY.md` | 3-tier journey system, 12-month plan |
| `docs/HANDBOOK.md` | Human-readable maintenance |
| `docs/HOW-IT-WORKS.md` | Founder explainer |
| `docs/lessons/` | Hard-learned rules |
