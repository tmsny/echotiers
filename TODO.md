# TODO – EchoTiers Overall Alias (admin-editierbar)

- [x] 1) `index.html` CSS ergänzen: Alias-Feld + Tooltip + Hover-Style + Border-Farbe aus DB
- [x] 2) Firebase-Datenmodell ergänzen:
  - [x] in `subscribePlayers()` `overallAliasText` / `overallAliasColor` laden (Fallback)
- [x] 3) Overall-Rendering anpassen in `renderOverallMode()`:
  - [x] Region-badge (NA-Feld) ersetzen durch Alias-Feld
  - [x] Default anzeigen: `overallAliasText` erste 3 Buchstaben
  - [x] Tooltip/Overlay bei Hover: vollständiger Alias-Text leicht über das Feld
- [x] 4) Admin-UI ergänzen in `renderOverallMode()`:
  - [x] klickbares Alias-Feld => Text Input + Farbauswahl (Select)
  - [x] Speichern via Button
- [x] 5) Event-Handler ergänzen (Admin save):
  - [x] `handleOverallAliasSave` (set player -> overallAliasText & overallAliasColor)
- [ ] 6) Funktion testen manuell:
  - [ ] Admin setzt Alias-Text + Farbe
  - [ ] Nicht-Admin sieht 3 Buchstaben + Tooltip


