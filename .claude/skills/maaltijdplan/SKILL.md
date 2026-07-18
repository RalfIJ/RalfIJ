---
name: maaltijdplan
description: Maakt een vegetarisch weekmenu rond de vier kookdagen (wo/vr/za/zo) met meal-prep voor de overige dagen, plus boodschappenlijst. Gebruik bij "weekmenu", "wat eten we", "maaltijdplan", "boodschappen", "meal prep", "recept", of /maaltijdplan.
---

# Maaltijdplanner

Maak een haalbaar vegetarisch weekmenu voor Ralf. Haalbaarheid gaat boven perfectie: een plan dat wordt uitgevoerd verslaat een perfect plan dat blijft liggen.

## Randvoorwaarden

- **Vegetarisch**, altijd.
- **Licht calorietekort zonder tellen**: stuur op porties en slimme defaults, niet op calorieën. Geen crashdieet, nooit maaltijden overslaan als strategie.
- **Eiwit prioriteit**: elke maaltijd één duidelijke eiwitbron; streef ~110-125 g/dag (praktisch, niet gemeten).
- Kookdagen: **alleen wo/vr/za/zo**. Ma/di/do: opwarmen of <10 min.
- **2 personen**: zondag-batch = 6 porties (3 dagen × 2), woensdag dubbel = 4 porties. Schaal de receptporties uit `referentie/recepten.md` hierop.
- **Psoriasis-vriendelijke defaults** (zachte voorkeur): veel groente/fruit, peulvruchten, volkoren, olijfolie, noten; weinig sterk bewerkt voedsel. Meldt Ralf zelf een persoonlijke trigger, respecteer die dan in alle volgende menu's.
- **Kaas: alleen mild** — geraspte kaas, cheddar, mozzarella, parmezaan als strooikaas. Nooit halloumi, brie, geitenkaas, feta of roomkaas programmeren.

## De kookdag-strategie (kern)

| Dag | Aanpak |
|---|---|
| Zondag | Batch-koken `[batch]`-recept, 3 porties → zo + ma + di |
| Woensdag | Dubbele portie → wo + do |
| Vrijdag | Vers koken, mag leuk en uitgebreid `[vers]` |
| Zaterdag | Vers koken, mag leuk en uitgebreid `[vers]` |

Vrijdag en zaterdag zijn geniet-dagen — die houden het vol te houden. Donderdag-fallback als de woensdagportie op is: een `[snel <15 min]`-recept.

## Werkwijze

1. **Vraag eerst kort** (max 3 vragen, alleen wat nodig is): zin in iets specifieks deze week? Nog iets over van vorige week? Dagen dat je uit eten gaat of niet thuis bent?
2. **Lees `referentie/recepten.md`** en stel het menu samen: batch-recept voor zondag, dubbel-recept voor woensdag, twee verse recepten voor vr/za. Wissel af met vorige weken als die bekend zijn.
   - Wil Ralf iets dat niet in de bibliotheek staat? **Niet gokken**: zoek het recept op internet op (werkwijze van `/recept`: Nederlandse bronnen zoals ah.nl/allerhande) of verwijs naar `/recept` om het toe te voegen.
3. **Presenteer het weekmenu als tabel**: dag | avondmaal | bron (vers gekookt / batch / restje / snel). Noem ook de ontbijt/lunch-rotatie kort.
4. **Boodschappenlijst**: gegroepeerd per supermarktcategorie (groente & fruit / houdbaar / koeling / diepvries), gesplitst in **weekend-inkoop** en eventueel een kleine **midweek-aanvulling** (voor de verse vr/za-recepten).

## Winkels (zie ook CLAUDE.md)

- Standaardlijst = **Albert Heijn** (naast de deur). Alles wat AH niet of duur heeft: benoem het apart.
- **Indonesische toko**: eerste keus voor tempeh, tofu, sambal, kecap en verse kruiden — beter en goedkoper dan de supermarkt. Zet toko-items als apart lijstje.
- **DekaMarkt**: noem alleen als alternatief bij grote inkopen; geen aparte lijst.
- Bij twijfel over assortiment of voor Bonus-aanbiedingen: gebruik WebSearch/WebFetch op ah.nl. Niet elke week verplicht — alleen als het de lijst echt beter maakt.

## Guardrails

- Snacks niet verbieden — wijs op de snacklijst in `referentie/recepten.md` (kwark, noten, fruit) als slimme default.
- Supplementen: alleen de algemene opmerking dat **B12** bij vegetarisch eten het checken waard is (bespreken met huisarts). Geen andere supplement- of medische adviezen.
- Psoriasis: blijf bij algemene voedingspatronen (ontstekingsremmend eten, gezond gewicht); geen claims over specifieke voedingsmiddelen die flare-ups "genezen". Medische vragen → huisarts of dermatoloog.
- Uit eten of een keer afwijken is prima: het gaat om het weekgemiddelde, niet om één dag.

## Schrijft

Standaard **niets** — het weekmenu is chat-output. Alleen als Ralf expliciet vraagt het te bewaren: `data/weekmenus/JJJJ-Www.md`.
