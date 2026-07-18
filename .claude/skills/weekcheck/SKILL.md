---
name: weekcheck
description: Wekelijkse review; bekijkt trainingen, gewichtstrend en hoe de week voelde, en past het trainingsschema aan voor volgende week. Gebruik bij "weekcheck", "check-in", "hoe ging mijn week", "nieuwe week", "weekreview", of /weekcheck.
---

# Wekelijkse check-in

Houd het schema levend: elke week een korte review en kleine, onderbouwde aanpassingen. Een check-in duurt 3 minuten — geen enquête.

## Stap 1 — Lees de data

1. `data/gewicht.csv` — weekgemiddelde van deze week vs. vorige week.
2. `data/trainingen/` van de afgelopen 7 dagen — aantal sessies vs. gepland, RPE's, notities over vorm of ongemak.
3. `data/checkins.md` — de afspraken van vorige week.
4. `data/metingen.csv` — is de laatste meting >1 maand oud (of is er nog geen)? Herinner dan aan het meten.
5. `schema/trainingsschema.md` — huidige week en stand.

## Stap 2 — Stel maximaal 3 korte vragen

1. Energie deze week (1-5)?
2. Wat was het grootste obstakel (of ging alles goed)?
3. Iets wat pijn deed of tegenstond?

## Stap 3 — Beslisregels (voorspelbaar, in deze volgorde)

- **2+ sessies gedaan én RPE's ≤8 én geen klachten** → schemaweek +1 (progressie volgens het schema).
- **0-1 sessies of energie ≤2** → dezelfde week herhalen. Bespreek het obstakel en verlaag de drempel (kortere sessies, ander tijdstip, sessie C i.p.v. kracht). **Nooit** laten "inhalen" met extra sessies.
- **2 mindere weken op rij of aanhoudende vermoeidheid** → herstelweek: gewichten -30%, alleen wandelen op de loopband.
- **Week 4 afgerond** → genereer blok 2 in het schemabestand: zelfde sessiestructuur, herhalingsbereik 8-12 met dubbele progressie. Cardio bouwt door **zonder joggen** (Ralfs keuze): meer helling, kortere rustblokken, en optioneel het low-impact HIIT-circuit uit `referentie/oefeningen.md` als sessie C-variant.
- **Gewichtstrend >1 kg/week omlaag (2+ weken)** → advies iets ruimer te eten (bijv. grotere lunch), tempo terug naar 0,25-0,5 kg/week.
- **3+ weken vlak gewicht** → stel **één** concrete voedingsaanpassing voor (nooit meer dan één tegelijk), bijv. avondsnack vervangen door kwark.
- Bij pijnklachten: betreffende oefening vervangen door de makkelijkere variant uit `referentie/oefeningen.md`; bij aanhoudende pijn huisarts adviseren.

## Stap 4 — Schrijf de uitkomst

1. **`schema/trainingsschema.md`** (alleen deze skill mag dit bestand aanpassen):
   - Update het blok **"Huidige stand"**: weeknummer, volgende sessie, focus, en de actuele werkgewichten (uit de trainingslogs van deze week).
   - Voeg één regel toe aan de **Aanpassingenlog**-tabel onderin: datum | aanpassing | waarom.
2. **`data/checkins.md`**: voeg bovenaan (direct onder de titel) een blokje toe:

   ```
   ## JJJJ-MM-DD — week N
   - Sessies: X van 2-3 (A/B/C: …)
   - Gewicht: weekgemiddelde XX.X kg (±X.X vs. vorige week)
   - Energie: N/5 · Obstakel: …
   - Besluit: (week +1 / herhalen / herstelweek / blok 2)
   - Afspraak voor volgende week: …
   ```

## Toon

- Begin **altijd** met wat goed ging, hoe klein ook.
- Missers zijn informatie ("wat maakte het lastig?"), geen falen. 2 sessies is een geslaagde week.
- Sluit af met één concrete, haalbare afspraak voor volgende week — niet drie.
