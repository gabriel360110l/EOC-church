# E.O.C Church — Source Catalog

**Eastern Orthodox · Oriental Orthodox · Catholic**

This repository is a clean **catalog of open sources, GitHub repositories, and free APIs** for building apps or tools related to the three main Christian traditions:

- **Eastern Orthodox** (Greek, Russian, etc.)
- **Oriental Orthodox** (Coptic, Syriac, Armenian, Ethiopian, etc.)
- **Catholic** (Roman & Eastern Catholic)

## How to use this catalog

1. Browse the folders by tradition (or the `shared/` folder for content common to all three).
2. Each file lists sources with:
   - A short explanation of what it is
   - What you can extract from it (texts, calendars, prayers, etc.)
   - Direct links
3. When you build an app you can:
   - Fetch data **live** from the APIs / repos
   - Or **download and bundle** the data you need for offline use

Nothing in this repo stores the full texts. It only points you to the sources.

## Structure

```text
shared/                  ← Content shared by all three traditions
  bibles.md
  councils_and_canons.md
  church_fathers.md

eastern_orthodox/
  prayers_and_horologion.md
  calendar_and_saints.md

oriental_orthodox/
  agpeya_and_prayers.md
  calendar_and_synaxarium.md

catholic/
  liturgy_of_the_hours.md
  calendar.md

calendars/               ← Quick daily API endpoints
  daily_endpoints.md
```

## Important notes

- Prefer public-domain or clearly open sources.
- Always check the license of a repository or API before redistributing content.
- Some APIs are free but may have rate limits.
- For offline apps: download what you need during build time or first launch and cache it.

## Quick start examples

- Today's Eastern Orthodox readings & saints: `https://orthocal.info/api/gregorian/`
- Today's Catholic feast: `http://calapi.inadiutorium.cz/api/v0/en/calendars/default/today`
- Coptic Synaxarium (example): `https://api.coptic.io/api/synaxarium/2026-10-17`

---

*This catalog was built to support the creation of high-quality, tradition-aware apps and tools.*
