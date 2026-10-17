# Daily Calendar & Readings Endpoints

Quick reference for “today” or date-specific data from the three traditions.

---

## Eastern Orthodox
- **Today:** https://orthocal.info/api/gregorian/
- **Specific date:** `https://orthocal.info/api/gregorian/YYYY/MM/DD/`
- **Returns:** Readings, saints, fasting rule, troparia.

---

## Oriental Orthodox (Coptic)
- **Synaxarium example:** `https://api.coptic.io/api/synaxarium/YYYY-MM-DD`
- **Agpeya hours:** `https://api.coptic.io/api/agpeya/prime` (also terce, sext, none, vespers, compline, midnight)

---

## Catholic
- **Today:** http://calapi.inadiutorium.cz/api/v0/en/calendars/default/today
- **Returns:** Feast, color, rank, and celebrations.

---

## Tips
- Most of these APIs do **not** require an API key.
- Cache responses in your app if you want offline support.
- Always check the current status of the endpoint before relying on it in production.
