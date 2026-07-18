---
name: logboek
description: Logt gewicht, lichaamsmetingen en trainingen in de data-bestanden en toont voortgangstrends. Gebruik bij "ik weeg", "gewicht loggen", "meting", "voortgang", "trend", "grafiek", "hoe gaat het met mijn gewicht", of /logboek.
---

# Voortgangslogboek

Eén laagdrempelige ingang voor alles wat gelogd wordt, plus trendweergave. Loggen moet in seconden kunnen — geen onnodige vragen.

## Loggen — herken uit vrije tekst wat bedoeld wordt

### Gewicht ("ik weeg 83.4", "83,4 vanochtend")
- Append één regel aan `data/gewicht.csv`: `datum,gewicht_kg,notitie` (notitie mag leeg).
- Decimalen met een **punt**, datum vandaag tenzij anders gezegd.
- Bestaat er al een regel met dezelfde datum → vraag: vervangen of laten staan?
- Bevestig kort en noem meteen het lopende 7-daags gemiddelde als er genoeg data is.

### Lichaamsmetingen ("taille 96", "ik heb gemeten")
- Append aan `data/metingen.csv`: `datum,taille_cm,heup_cm,borst_cm,bovenarm_cm,notitie` — velden die niet gemeten zijn blijven leeg.
- Geef bij de eerste keren de meetinstructie: 's ochtends, ontspannen (niet inhouden), taille op navelhoogte, meetlint horizontaal.
- Metingen zijn maandelijks zinvol, vaker niet.

### Training achteraf ("ik heb gisteren getraind, vergeten te loggen")
- Schrijf `data/trainingen/JJJJ-MM-DD.md` volgens het format van `data/trainingen/VOORBEELD.md` (tabel: Oefening | Sets × herh | Gewicht (kg) | RPE). Vraag alleen naar wat ontbreekt.

**Alle CSV's zijn append-only**: wijzig nooit historische rijen zonder dat Ralf er expliciet om vraagt.

## Trends tonen ("hoe gaat het", "voortgang", "trend")

Parse `data/gewicht.csv` (en `data/metingen.csv` als er data is) en toon:

1. **Huidig 7-daags gemiddelde** vs. vorige week vs. startgewicht (84,0 kg).
2. **Totaal verschil sinds start** en het gemiddelde tempo per week.
3. Een compacte **weektabel** in tekst (week | gemiddeld gewicht | verschil). Een grafiekbestand alleen als Ralf er expliciet om vraagt.
4. Als er metingen zijn: verschil in taille-omtrek sinds start (vaak eerlijker dan de weegschaal).

## Interpretatie-guardrails

- Oordeel **alleen op weekgemiddelden** — dagschommelingen van ±1-2 kg zijn vocht en maaginhoud, geen vet.
- Verlies **>1 kg/week gedurende 2+ weken** → vlag: "dit gaat te snel, eet iets ruimer" (streef is 0,25-0,5 kg/week).
- Stagnatie korter dan **3 weken** is geen plateau — nog niets aanpassen.
- Weegschaal is niet de enige maat: sterkere trainingen en een kleinere taille zijn óók voortgang, zeker bij een beginner die spier opbouwt.
- Nooit veroordelend over een stijging; benoem het neutraal en kijk naar de weektrend.

## Weegritme-advies (op verzoek)

Dagelijks óf 2-3× per week, maar altijd op een vast moment: 's ochtends, na het toilet, vóór het ontbijt. Kies wat vol te houden is.
