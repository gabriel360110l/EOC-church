# Bijbel Quizzen

Gedetailleerde uitleg van het quiz-systeem voor de app.

## Doel
Gebruikers moeten na het lezen van een hoofdstuk of een leesdag een korte quiz maken. Alleen als ze de quiz goed genoeg maken, kunnen ze verder naar het volgende hoofdstuk of de volgende dag van het plan.

Dit zorgt ervoor dat mensen de tekst echt lezen en onthouden, in plaats van alleen maar door te scrollen.

## Hoe het werkt (stap voor stap)

1. Gebruiker leest een hoofdstuk (of de lezingen van een dag in een plan).
2. Aan het einde verschijnt een knop “Quiz starten”.
3. De quiz bevat 5–10 meerkeuzevragen over de gelezen tekst.
4. Gebruiker beantwoordt de vragen.
5. Score wordt berekend.
6. **Als de score hoog genoeg is** (bijv. 70% of 80%):
   - Hoofdstuk/dag wordt als “voltooid” gemarkeerd.
   - Volgende hoofdstuk of volgende dag van het plan wordt ontgrendeld.
7. **Als de score te laag is**:
   - Gebruiker krijgt te zien welke vragen fout waren + korte uitleg.
   - Mag de quiz opnieuw doen (eventueel na een korte wachttijd of direct).

## Twee niveaus

### A. Quiz per hoofdstuk
- Na elk hoofdstuk (Genesis 1, Matteüs 5, etc.).
- Korte quiz, alleen over dat hoofdstuk.
- Ideaal om te voorkomen dat mensen hoofdstukken overslaan.

### B. Quiz aan het einde van een leesdag (bij een plan)
- Na alle lezingen van die dag.
- Vragen over de verschillende gedeelten die die dag gelezen zijn.
- Handig bij plannen die meerdere passages per dag hebben.

### C. Quiz aan het einde van een boek (optioneel)
- Grotere quiz over het hele boek.
- Kan als extra uitdaging of als vereiste om een boek “af te ronden”.

## Score en ontgrendeling

- Aanbevolen drempel: **70–80% goed**.
- Bij een te lage score: uitleg bij foute antwoorden + mogelijkheid om opnieuw te proberen.
- Voortgang wordt lokaal opgeslagen (zodat de gebruiker niet steeds opnieuw hoeft te beginnen).
- Optioneel: een “skip” na meerdere mislukte pogingen (voor mensen die vastlopen), maar standaard is de quiz verplicht.

## Inhoud van de quizzen

Vragen kunnen gaan over:
- Wat er gebeurde in het hoofdstuk
- Belangrijke personen
- Centrale boodschap of les
- Verband met andere gedeelten (vooral bij OT–NT gekoppelde plannen)
- Optioneel: wat een kerkvader over dit gedeelte heeft gezegd

## Bronnen voor vragen

- Zelf geschreven vragen (beste kwaliteit).
- Bestaande open datasets (zoek op GitHub naar “bible quiz json” of “bible questions”).
- Gegenereerde vragen op basis van de tekst (met controle).

## UI-aanbevelingen

- Duidelijke knop na het lezen: “Maak de quiz om verder te gaan”.
- Voortgangsbalk tijdens de quiz.
- Na afloop: score + uitleg bij foute antwoorden.
- Visuele feedback: groen vinkje als een hoofdstuk/dag voltooid is.
- In het leesplan: vergrendelde dagen/hoofdstukken tonen met een slot-icoon.

## Technische opmerkingen

- Sla de status per hoofdstuk of per dag op (bijv. “genesis_1_completed”: true).
- Houd bij hoeveel pogingen iemand heeft gedaan.
- Maak de quizzen kort genoeg dat ze niet frustrerend worden.
- Test de vragen goed, zodat er geen onduidelijke of foute vragen in zitten.

## Samenvatting

| Onderdeel          | Aanbeveling                     |
|--------------------|---------------------------------|
| Wanneer            | Na hoofdstuk of na leesdag      |
| Aantal vragen      | 5–10                           |
| Slagingspercentage | 70–80%                        |
| Bij falen          | Uitleg + opnieuw proberen       |
| Doel               | Echt lezen en onthouden         |

Dit systeem maakt de leesplannen actiever en zorgt ervoor dat gebruikers de Bijbel beter begrijpen en onthouden.
