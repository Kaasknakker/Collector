# Collector 0.2 (versie Claude)

Onafhankelijke 0.2, gebouwd zonder de ChatGPT-versie als uitgangspunt. Alleen deze map is nieuw; `main` en 0.1 zijn niet aangeraakt.

## De ene verandering
**Land heeft pas waarde als je water afsluit.** In 0.1 maakte plaatsing niets uit. Nu legt het voertuig een dijk en pas als een stuk zee helemaal omsloten is (kust tot kust, of een ring), wordt het drooggemalen en krijg je geld naar oppervlakte. Een korte dijk die veel water afsluit is dus veel beter dan een lange kronkel. De vorm is de keuze.

## Bediening
- **Tik** = rijden (legt nooit een dijk).
- **Vinger vasthouden en slepen** (langer dan 0,2 s) = dijk leggen terwijl je rijdt. Loslaten: het voertuig maakt de laatste meters nog af.
- Tik op het voertuig = stoppen.
- Laden gaat vanzelf in de zandput (altijd ongeveer 1 seconde, onafhankelijk van capaciteit).
- Eén dijkstuk kost één eenheid zand. Een halve dijk blijft staan als het zand op is.

## Eerlijkheidsfixes t.o.v. 0.1 (geen nieuwe features)
- Capaciteit doet nu echt iets (langere dijk per lading) en was in 0.1 een placebo.
- Snelheid is een echte upgrade (het voertuig rijdt zichtbaar sneller) en zit niet vast aan een vaste stortduur.
- Geen knoppen om ingedrukt te houden; alles kan met één duim.
- Land stijgt zichtbaar: dijk met pop-animatie, droogmaalgolf van de rand naar binnen, belletjes-ring, munten en bedrag.
- Eén tekenlus (in 0.1 kwamen er bij elke resize lussen bij).

## Test
- Gebruik 5 mensen die het niet kennen, 10 minuten, zonder uitleg.
- Laat het testoverzicht zien met **5x tikken op "Collector 0.2"**: tijd tot eerste zand, eerste dijkstuk en eerste polder, aantal polders, dijkstukken, upgrades en een tijdlijn. "Nieuw spel" staat daar ook.
- Kijk vooral naar: zoeken ze zelf naar een beter plan of doen ze allemaal hetzelfde? Reageren ze op het sluiten? Beginnen ze uit zichzelf aan een tweede polder?

## Verwerp als
Meer dan de helft afhaakt binnen 4 minuten, niemand een tweede polder begint, of iedereen dezelfde simpele strategie volgt.

## Afstellen (bovenin `index.html`)
`START_CAP`, `CAP_STEP`, `LOAD_TIME`, `BASE_SPEED`, `CELL_VALUE`, `PUMP_DUR` en `PROFILE` (de kustlijn).
