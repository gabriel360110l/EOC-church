# How to Use This Catalog in an App

## 1. Live data (simplest)
Your app calls the API endpoints listed in this repo when the user needs content.

Example (Eastern Orthodox today):
```
GET https://orthocal.info/api/gregorian/
```

## 2. Offline / bundled data
1. During development or in a build script, download the files or API responses you need.
2. Save them as JSON inside your app’s `assets/` folder or in a local database.
3. The app then reads from the local files when offline.

## 3. Hybrid (recommended)
- Bundle the most important static content (creeds, core prayers, main canons).
- Fetch daily content (saints, readings, variable prayers) live and cache it for a few days.

## License reminder
Before you redistribute any text in your app:
- Prefer public-domain sources (WEB, Statenvertaling, NPNF, etc.).
- Check the license of each GitHub repository.
- For APIs, respect their terms of use and rate limits.

## Suggested starting points for an app

| Feature                  | Best source                          |
|--------------------------|--------------------------------------|
| English Bible            | WEB (helloao or ebible)              |
| Dutch Bible              | Statenvertaling + Apocrypha or Canisius |
| Daily EO readings/saints | orthocal.info                        |
| Coptic Agpeya            | api.coptic.io                        |
| Catholic Hours           | breviarium--core or liturgy-day      |
| Early Councils & Canons  | npnf214.xml                          |
| Verse commentaries       | Commentaries-Database (select books) |

---

This catalog is meant to save you time finding good sources. Start small, add more sources as your app grows.
