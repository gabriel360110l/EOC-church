# Bijbelverzen koppelen aan Kerkvader-commentaren

Dit is een van de sterkste features die je app kan hebben: bij elk vers laten zien wat de heiligen en kerkvaders erover hebben gezegd.

## De beste bron

**HistoricalChristianFaith/Commentaries-Database**

- Link: https://github.com/HistoricalChristianFaith/Commentaries-Database
- Staat ook beschreven in `shared/church_fathers.md`
- Elk vers heeft een eigen JSON-bestand (voorbeeld: `jn/1/1.json` voor Johannes 1:1)
- Bevat commentaren van o.a. Johannes Chrysostomus, Athanasius, Cyrillus van Alexandrië, Efrem de Syriër, Augustinus, Basilius de Grote, Gregorius van Nazianze, etc.
- Ook deuterocanonieke boeken zitten erin (Tobit, Wijsheid, Sirach, Makkabeeën, etc.)

### Voorbeeldstructuur van een vers-bestand
Een bestand bevat meestal een array van commentaren met:
- Naam van de vader
- Jaar / periode
- De tekst van het commentaar
- Soms een verwijzing naar het werk (homilie, brief, etc.)

## Hoe je het in de app implementeert

### Optie A — Live ophalen (eenvoudig starten)
1. Gebruiker opent een vers.
2. App bouwt de URL op basis van boek + hoofdstuk + vers.
3. Haalt het JSON-bestand op van de GitHub raw-link of via een eigen cache.
4. Toont de commentaren.

**Voordeel:** altijd up-to-date, weinig opslag.  
**Nadeel:** internet nodig.

### Optie B — Offline bundelen (aanbevolen voor productie)
1. Download tijdens de ontwikkeling alleen de boeken die je wilt (bijv. de Evangeliën + Psalmen + belangrijkste deuterocanon).
2. Zet de JSON-bestanden in de app (assets of lokale database).
3. App leest lokaal.

**Voordeel:** werkt offline, snel.  
**Nadeel:** app wordt groter (selectief downloaden houdt het beheersbaar).

### Optie C — Hybride
- Belangrijkste boeken offline.
- Overige boeken live ophalen en cachen.

## UI-aanbevelingen

- Bij elk vers een subtiele knop of icoon: “Kerkvaders” of een klein heiligen-icoon.
- Tikken opent een bottom sheet of nieuw scherm met de commentaren.
- Toon per commentaar:
  - Naam van de vader (vet)
  - Korte periode (bijv. “4e eeuw”)
  - De tekst
  - Optioneel: “Lees meer” als er een link naar het volledige werk is
- Groepeer eventueel op vader of op chronologische volgorde.
- Als er geen commentaar is: toon niets of een korte melding “Geen commentaar beschikbaar voor dit vers”.

## Extra mogelijkheden

- Filter op traditie (alleen pre-451 vaders voor gedeelde content, of specifiek Eastern / Oriental / Catholic).
- Link vanuit een commentaar naar de volledige tekst in de Writings-Database (ook van HistoricalChristianFaith).
- Markeer favoriete commentaren of vaders.
- Toon een klein icoon van de vader als je die hebt (Byzantijnse stijl).

## Technische tips

- Normaliseer boeknamen (bijv. “Jn”, “John”, “Johannes” → zelfde code).
- Cache agressief als je live ophaalt.
- Test met bekende verzen die veel commentaar hebben (Johannes 1:1, Matteüs 5, Psalmen, etc.).
- Respecteer de licentie van de database (check de repo).

## Samenvatting

| Onderdeel              | Aanbeveling                          |
|------------------------|--------------------------------------|
| Bron                   | Commentaries-Database                |
| Opslag                 | Selectief offline + cache            |
| UI                     | Knop bij vers → lijst van vaders     |
| Extra                  | Link naar volledige tekst indien mogelijk |

Dit maakt de app uniek en diepgaand zonder dat je zelf alle commentaren hoeft te schrijven.
