# Bible Cross-References

Cross-references laten zien welke verzen in de Bijbel met elkaar verbonden zijn (zelfde thema, citaat, vervulling, personen, etc.).

---

## Beste bron: CrossReferences-org / bible-cross-references

- **Wat het is:**  
  Open dataset gebaseerd op de klassieke *Treasury of Scripture Knowledge*. De references zijn gekoppeld aan **specifieke woorden of zinnen** in een vers (niet alleen vers → vers).

- **Wat je eruit haalt:**  
  Schone JSON-bestanden waarmee je in een app kunt laten zien:  
  “Dit woord/deze zin in dit vers verwijst naar deze andere verzen.”

- **Link:**  
  https://github.com/CrossReferences-org/bible-cross-references

- **Belangrijkste bestanden:**
  - `bible_books.json` — lijst van boeken
  - `bible_verses.json` — alle verzen met tekst
  - `cross_references.json` — de eigenlijke cross-references per vers

- **Licentie:** CC BY 4.0 (vrij te gebruiken, wel bron vermelden)

- **Ondersteunde vertalingen:** KJV, Berean Standard Bible, en meer.

### Hoe je het in een app gebruikt
1. Download de JSON-bestanden (of een deel ervan).
2. Zet ze offline in de app of cache ze.
3. Wanneer de gebruiker een vers opent:
   - Zoek of er cross-references zijn voor dat vers.
   - Toon een knop of markeer het woord in de tekst.
   - Bij tikken: toon de gerelateerde verzen (met korte tekst).
   - Tikken op een gerelateerd vers opent dat vers.

### Voorbeeld (vereenvoudigd)
```json
{
  "verse_id": 10,
  "kjv": "beginning",
  "refs": [
    [261190, 261200, 261210],
    [300490]
  ]
}
```
Dit betekent: het woord “beginning” in dit vers verwijst naar andere verzen.

---

## Andere nuttige bronnen

### neuu-org / bible-crossrefs-dataset
- **Wat het is:** Grote gecombineerde set (OpenBible + Treasury of Scripture Knowledge).
- **Wat je eruit haalt:** Meer dan 1,1 miljoen cross-references in verschillende formaten.
- **Link:** https://github.com/neuu-org/bible-crossrefs-dataset
- **Beste voor:** Als je een maximale hoeveelheid references wilt.

### scrollmapper / bible_databases
- **Wat het is:** Grote verzameling Bijbelteksten + cross-references.
- **Wat je eruit haalt:** Cross-references (van OpenBible) samen met veel Bijbelvertalingen in SQLite/JSON.
- **Link:** https://github.com/scrollmapper/bible_databases
- **Beste voor:** Als je toch al Bijbelteksten uit deze repo haalt.

---

## Aanbeveling voor de app

Gebruik **CrossReferences-org/bible-cross-references** als hoofdbron.  
De phrase-level koppeling maakt het veel nuttiger dan alleen “vers A verwijst naar vers B”.

Je kunt het combineren met:
- De Bijbeltekst (uit `shared/bibles.md`)
- Kerkvader-commentaren (uit `shared/church_fathers.md`)
