# Offline Strategie

De app moet zo veel mogelijk offline werken.

## Wat offline moet kunnen
- Bijbeltekst (minimaal één vertaling)
- Gebeden (Agpeya, Horologion, vaste gebeden)
- Heiligen van de dag (basisinfo)
- Kerkvader-commentaren (voor de belangrijkste boeken)
- Leesplannen en quizzen
- Eerder gelezen voortgang

## Aanpak
1. **Bij eerste installatie of eerste keer openen**  
   Download de kern-data (Bijbel + belangrijkste gebeden) en sla die lokaal op.

2. **Selectief downloaden**  
   Laat de gebruiker extra vertalingen, extra boeken of commentaren downloaden wanneer hij wil.

3. **Cache**  
   Dagelijkse content (heiligen, lezingen) wordt gecachet voor een aantal dagen.

4. **Updates**  
   Controleer af en toe of er nieuwe data is, maar forceer geen download.

## Technische tips
- Gebruik een lokale database (SQLite) of JSON-bestanden in de app.
- Toon duidelijk wanneer iets offline beschikbaar is.
- Bij geen internet: gebruik de lokale data en geef een vriendelijke melding als iets niet beschikbaar is.
