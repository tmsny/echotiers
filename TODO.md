# Echotiers – TODO

## Ziel
Separate Ansichten für **Current** und **Prime** pro Modus (Option B), mit Regel:
- **alle Current-Modi** werden bei **Overall-Current** gepunktet
- **Prime** wird bei **Overall-Prime** gepunktet

## Schritte
1. Repo-Stand prüfen: `index.html` (bestehende Render-/Filter-Logik für overall & mode table).
2. (Done) State-Grundlage angepasst: `tierlistMode` wird als UI-Selektor verstanden.
3. Plan bestätigen: UI-Rendering in `renderPlayers()` so umbauen, dass pro Modus zwei Sections gerendert werden (Current & Prime), insgesamt 18 Sections.
4. Berechnungspfade anpassen:
   - `getPlayerTotalPoints(player, tierlistMode)` so erweitern, dass Overall-Points korrekt aus Current bzw Prime Tiers gezogen werden.
   - `getPlayerTotalPoints`-Callsites in Overall Current/Prime und Modal anpassen.
5. Rendering anpassen:
   - `renderOverallMode` in zwei Teil-Renderings aufteilen.
   - `renderModeTable` ebenfalls in zwei Teil-Renderings (Current/Prime) aufteilen.
6. Admin/Swap Logik prüfen:
   - Tier-Selects müssen weiterhin auf den richtigen Pfad schreiben (tiers vs primeTiers), aber Shift- bzw Swap in korrektem Sub-Mode/Overall-Sub-Ansicht laufen.
7. Event-Listener/State:
   - `tierlistMode` Switch ggf. nur noch für Selected-UI nutzen oder durch festes Rendering (current+prime) ersetzt.
8. Testlauf im Browser: Filter, Search, Prime/Current Anzeige, Modal-Tiers, Admin-Save/Swap.


