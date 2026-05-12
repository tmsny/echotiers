# TODO – EchoTiers cracked + Slash-Handling

- [ ] 0) Parser einbauen: `rawName` → `{ name, cracked }` (leading `/` => cracked, Name ohne `/`)
- [ ] 1) `addNewPlayer()` updaten: Name/ID/DB speichern (inkl. `cracked`)
- [ ] 2) `subscribePlayers()` updaten: `cracked` aus DB laden (fallback false für alte Daten)
- [x] 3) Rendering Tierlist: Badge (klein) neben dem Spielernamen anzeigen, ohne Sortierung/Filter zu ändern
- [x] 4) Rendering Modal/Profile: Badge (klein) anzeigen, Skin/NameMC korrekt über `player.name`

- [ ] 5) Optional: Seed-Sample kompatibel (cracked=false bei fehlendem Feld)
- [x] 6) Manuell testen: /Lukas, Lukas, Alt-Daten

