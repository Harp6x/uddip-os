# Aishani Content — Project Summary

**Repo:** `Harp6x/aishani-content` | **Local:** `~/Documents/aishani`

---

## Mission
Complete content engine for Ms Paul Therapies — everything Aishani needs to run Instagram, YouTube, blog, email, client work, and digital products. All in one place.

## Audience
Internal — used by Aishani Paul for her therapy practice content. The README includes a non-technical guide for Aishani to navigate the repo directly on GitHub.

## Business Model
Not revenue-generating directly. Supports Ms Paul Therapies content marketing, digital products, and client resources.

## Technology
Pure markdown repository. 722 markdown files + 10 branded PDFs, with lightweight scripts/workbook templates for PDF and practice operations. Generated handbook output lives in `_generated-handbooks/`.

## Structure
```
├── content/              → Blog articles, reel scripts, carousel scripts, series outlines
├── digital-products/     → Workbooks, worksheets, guides for clients
├── checklists/           → Clinical and business checklists
├── questionnaires/       → Assessment tools
├── guides/               → How-to guides
├── workbooks/            → Therapy workbooks
├── worksheets/           → Client worksheets
├── scripts/              → Video/reel scripts
├── growth-playbook/      → Marketing strategy and growth plans
├── execution-playbook/   → Execution plans
├── mspaultherapies/      → Website-specific content
├── pdfs/                 → Branded downloadable PDFs
├── business-setup/       → Business infrastructure docs
├── client-operations/    → Client management processes
├── revenue-infrastructure/ → Revenue planning
├── learning/             → Professional development
├── _knowledge-expansion/ → Knowledge base expansion
├── _life-architecture/   → Personal systems
├── _strategic-audit/     → Business audits
├── Planner/              → Planning documents
└── _generated-handbooks/ → Generated Aishani Life & Practice OS handbook
```

## Roadmap
1. Continuous content creation (blog, social, digital products)
2. Monthly publishing cadence for Instagram + blog
3. Launch 2 digital products (Q3)
4. Workshop content development (Q4)
5. Use the generated Aishani handbook as the practice/content/product/revenue/life OS review surface

## Dependencies
- **Ms Paul Therapies** — All content feeds the therapy website
- **GitHub** — Version control
- **Uddip Content generator** — `~/Documents/uddip content/tools/build_uddip_multi_handbooks.py --profile aishani`

## Relationship to Other Projects
- 1:1 content source for Ms Paul Therapies website
- Content flows: Aishani Content → Sanity CMS → mspaultherapies.in
- Similar structure to Uddip Content (shared `_os/` patterns)
- No relationship to Before Maps or Hobie

## Documentation
| Doc | Purpose |
|---|---|
| `README.md` | Repo overview + non-technical guide for Aishani |
| `SITEMAP.md` | Complete file listing |
| `_generated-handbooks/README.md` | Generated handbook index + source ledger |
| `_generated-handbooks/01-AISHANI-LIFE-AND-PRACTICE-OS-HANDBOOK.md` | Master Aishani practice and life OS |
