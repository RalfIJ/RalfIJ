---
name: recept
description: Zoekt nieuwe vegetarische, eiwitrijke recepten op internet en voegt ze na goedkeuring toe aan de receptenbibliotheek. Gebruik bij "nieuw recept", "recept zoeken", "iets anders eten", "inspiratie", "recept toevoegen", "recept van internet", of /recept.
---

# Recepten-skill

Zoekt nieuwe recepten voor de bibliotheek in `referentie/recepten.md`. Kernregel: **nooit een recept verzinnen of gokken — altijd van internet halen**, met bronvermelding.

## Stap 1 — Wat zoekt Ralf?

Vraag alleen wat nog niet duidelijk is (max 2 vragen):
- Type gerecht of ingrediënt ("iets met tempeh", "een ovenschotel")?
- Voor welke slot: `[batch]` (zondag, moet 6 porties aankunnen en goed bewaren), `[vers]` (vr/za, mag uitgebreider) of `[snel <15 min]` (doordeweekse fallback)?

## Stap 2 — Zoek op internet (verplicht, nooit gokken)

- Gebruik **WebSearch/WebFetch** op Nederlandse bronnen. Eerste keus: **ah.nl/allerhande** (AH is de standaardwinkel, ingrediënten dus altijd verkrijgbaar). Daarnaast bijv. Lekker en Simpel, 15gram, Uit Pauline's Keuken.
- Benut de **Indonesische toko** actief: recepten met tempeh, tofu, sambal en kecap zijn goedkoop, eiwitrijk en dichtbij verkrijgbaar.
- Haal het echte recept op (ingrediënten + bereiding), niet alleen de titel.

## Stap 3 — Harde filters (alles moet kloppen)

1. **Vegetarisch** (let op verstopte vis-/vleesbouillon of vissaus — vervang of skip).
2. **Eiwitrijk**: ≥20 g eiwit per portie voor avondmaaltijden. Net te laag? Stel een aanvulling voor (extra tofu, ei, bonen, kwark toe) en vermeld dat expliciet.
3. **Kaas alleen mild**: geraspte kaas, cheddar, mozzarella, parmezaan als strooikaas. Recepten met halloumi, brie, geitenkaas, feta of roomkaas: overslaan of de kaas vervangen (en dat benoemen).
4. **Psoriasis-voorkeur** (zacht): voorkeur voor veel groente, peulvruchten, volkoren, olijfolie; liever niet zwaar bewerkt of frituur als hoofdmoot.
5. **Haalbaar**: past bij de kookdag-strategie en het niveau "makkelijk, geen moeilijke technieken".

## Stap 4 — Presenteer 2-3 opties

Per optie compact: naam · bron-URL · geschat eiwit p.p. · tag (`[batch]`/`[vers]`/`[snel]`) · hoofdingrediënten · eventuele aanpassing (kaas vervangen, eiwit aangevuld).

## Stap 5 — Na goedkeuring: toevoegen aan de bibliotheek

- Append het gekozen recept aan de sectie **Avondrecepten** in `referentie/recepten.md`, in het bestaande format: volgnummer, naam + tag, porties + eiwit p.p., ingrediëntenregel, bereiding in 4-6 regels, en **de bron-URL** als laatste regel.
- Ontbijt/lunch-ideeën gaan in de rotatielijst bovenin datzelfde bestand.
- Dit is de **enige** schrijfactie van deze skill. Zonder goedkeuring niets opslaan.

## Toon

Kort en smakelijk — verkoop het gerecht in één zin, geen lappen tekst. Bij twijfel over een filter: benoem het eerlijk in plaats van het recept stilletjes aan te passen.
