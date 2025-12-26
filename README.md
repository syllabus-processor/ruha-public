# ruha-public

Public trust surface for ruha.io - static pages only.

## Purpose

This repo contains the public-facing legal and informational pages for EMA (Electronic Mental Health Application). These pages are intentionally separate from the clinical application (`ema-api`) to maintain clear trust boundaries.

## Contents

| File | URL | Purpose |
|------|-----|---------|
| `index.html` | https://ruha.io | Landing page |
| `privacy.html` | https://ruha.io/privacy | Privacy Policy |
| `terms.html` | https://ruha.io/terms | Terms & Conditions |

## Deployment

Deployed as a **Static Site** on DigitalOcean App Platform.

### Setup

1. Create new App in DO App Platform
2. Source: This GitHub repo
3. Type: Static Site
4. Build Command: (none)
5. Output Directory: `/`
6. Domain: `ruha.io`

### DNS

Configure DNS to point `ruha.io` (root) to the DO App Platform static site.

## Design Principles

- No JavaScript
- No analytics
- No cookies
- No tracking
- Plain HTML + inline CSS
- Mobile-responsive
- Fast loading
- HIPAA-aligned language
- Non-extractive tone

## What This Is NOT

This is NOT:
- A marketing site
- A sign-up funnel
- A feature showcase
- Part of the clinical application

## Relationship to Other Services

| Domain | Service | Repo |
|--------|---------|------|
| `ruha.io` | This static site | ruha-public |
| `ema.ruha.io` | Clinical app | ema-api (client) |
| `api.ruha.io` | API | ema-api |
| `auth.ema.ruha.io` | Auth | auth-service |

## Updates

Updates to these pages should be:
- Minimal
- Compliance-driven
- Approved by CTO

Do not add features, animations, or marketing language.

---

**Created:** December 2025
**Owner:** John Surmont (CTO)
