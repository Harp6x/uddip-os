# Uddip Content — Project Summary

**Repo:** `Harp6x/uddip-content` | **Local:** `~/Documents/uddip content`

---

## Mission
Complete content library powering three creator brands: HARP6X (systems lab), ThereGoesUddip (field journal), and Before Maps (travel company). Single repo, editorially separate brands.

## Audience
Internal — used by Uddip to publish across all platforms and brands.

## Business Model
Not revenue-generating directly. Supports content marketing, digital product creation, and brand building for all three brands.

## Technology
Pure markdown repository with one handbook generator script. 3,270+ markdown files organized by brand and function, plus generated operating handbooks in `_generated-handbooks/`.

## Structure
```
├── harp6x/              → AI, cybersecurity, creator systems, productivity
├── theregoesuddip/      → Solo travel, Himalayan treks, slow travel, essays
├── before-maps/         → Journey content, scouting reports, field notes (1,250+ pieces)
├── _os/                 → Operating system docs, calendars, strategy
├── _common/             → Shared templates, formats
├── automation/          → Workflow automation templates
├── cms/                 → CMS content ready for seeding
├── consultant-playbook/ → Consulting frameworks
├── crossover/           → Cross-brand content opportunities
├── digital products empire/ → Product blueprints, launch plans
├── execution/           → Execution frameworks
├── funnels/             → Marketing funnel designs
├── launch/              → Launch playbooks
├── learning/            → Learning resources, courses
├── life-architecture/   → Personal systems
├── personal-docs/       → Personal documents
├── proof/               → Social proof, case studies
├── shared/              → Shared assets
├── travel-startup/      → Travel business planning
├── Planner/             → Planning documents
├── tools/               → Handbook generator
└── _generated-handbooks/ → Generated Uddip operating handbook set
```

## Roadmap
1. Continuous content creation
2. 90-day content calendar execution
3. Before Maps content seeding into Sanity CMS
4. Digital product launches (HARP6X brand)
5. Keep generated handbooks current using `tools/build_uddip_multi_handbooks.py --profile uddip`

## Dependencies
- **Before Maps** — `before-maps/` folder feeds the Before Maps website
- **GitHub** — Version control and collaboration
- **Aishani Content** — same generator can build Aishani's generated handbook via `--profile aishani`

## Relationship to Other Projects
- `before-maps/` folder directly feeds Before Maps Sanity CMS
- `harp6x/` and `theregoesuddip/` are independent brands
- Strategic docs in `_os/` inform decisions across all projects
- Similar structure/philosophy to Aishani Content repo

## Documentation
| Doc | Purpose |
|---|---|
| `README.md` | Repo overview, brand descriptions, structure |
| `SITEMAP.md` | Complete file listing |
| `_os/` | Operating system, strategy, calendars |
| `_generated-handbooks/README.md` | Generated handbook index + source ledger |
| `_generated-handbooks/05-EXECUTION-REVENUE-COMMAND-CENTER.md` | Recommended execution-first handbook |
| `FOUNDER-STRATEGIC-REVIEW.md` | Multi-business audit |
