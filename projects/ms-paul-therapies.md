# Ms Paul Therapies — Project Summary

**Repo:** `Harp6x/misspaultherapies` | **Local:** `~/Documents/code/miss-paul-therapies`
**Live:** mspaultherapies.in | **Sanity:** k0r3y2my

---

## Mission
Professional online therapy practice for Aishani Paul — RCI-licensed clinical psychologist. Lead generation + educational content platform. NOT a booking engine.

## Audience
Indian adults (25–45) seeking mental health support — professionals, couples, parents, students. Also NRIs abroad.

## Business Model
- Therapy sessions (per-session fee via Cal.com booking)
- Digital products (workbooks, worksheets, guides on Gumroad)
- Workshops (group workshops, webinars — occasional)
- Newsletter (Kit/ConvertKit)

## Technology
Next.js 16.2.6 (App Router) · TypeScript · React 19 · Sanity v5 (12 document types) · Tailwind CSS v4 (sage/cream/terracotta palette) · Google Forms + Cal.com · Kit newsletter · Vercel

## Roadmap
1. Content updates via Aishani Content repo
2. SEO monitoring and improvement
3. Launch 2 digital products (Q3)
4. Workshop series (Q4)

## Dependencies
- **Aishani Content** — All content sourced from this repo
- **Sanity CMS** — Editorial content management
- **Cal.com** — Appointment scheduling
- **Google Forms** — Intake forms
- **Kit (ConvertKit)** — Newsletter

## Relationship to Other Projects
- Shares Next.js + Sanity + Tailwind architecture with Before Maps
- Content sourced from Aishani Content repo
- Aishani Paul is Uddip's partner — separate brand, separate audience
- No cross-promotion with Before Maps or Hobie

## Key Technical Notes
- **Dual-source data:** Sanity-first with static file fallback (`src/content/*.ts`)
- **Homepage mostly hardcoded:** Pain points, how-it-works, trust badges are arrays in `page.tsx`
- **No dark mode:** Fixed warm cream/sage/terracotta palette
- **No write client:** Sanity is read-only. Forms go through Google Forms + Cal.com
- **SEO-heavy:** 10+ JSON-LD builders, sitemap, robots, `llms.txt`
- **Blog fallback:** `src/content/blog.ts` is 40KB with 60+ posts

## Documentation
| Doc | Purpose |
|---|---|
| `CLAUDE.md` | AI standalone context |
| `AGENTS.md` | Full AI context (299 lines) |
| `MASTER-RCA.md` | Complete technical + marketing docs |
| `docs/ARCHITECTURE.md` | System architecture |
| `docs/HANDBOOK.md` | Maintenance guide |
| `docs/HOW-IT-WORKS.md` | Founder explainer |
| `docs/lessons/` | Hard-learned rules |
