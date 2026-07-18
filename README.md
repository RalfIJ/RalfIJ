# Fitness-toolbox

Persoonlijke fitness-coach als Claude Code toolbox. Open een Claude-sessie in deze repo en gebruik:

| Command | Wanneer |
|---|---|
| `/training` | Als je gaat trainen — stelt de sessie van vandaag voor en begeleidt je |
| `/maaltijdplan` | Begin van de week — vegetarisch weekmenu + boodschappenlijst |
| `/logboek` | Even iets loggen ("ik weeg 83.4") of je voortgang bekijken |
| `/weekcheck` | Zondagavond — weekreview, past het schema aan |

Je kunt ook gewoon typen wat je wilt ("ik ga zo trainen", "wat eten we deze week") — de juiste skill triggert vanzelf.

## Hoe het werkt

- `CLAUDE.md` — jouw profiel en de spelregels (apparatuur, kookdagen, veiligheidsprincipes).
- `schema/trainingsschema.md` — het actuele schema; wordt wekelijks bijgestuurd door `/weekcheck`.
- `data/` — je logs (gewicht, metingen, trainingen, check-ins). Platte tekst, dus je kunt er altijd zelf in kijken of iets aanpassen.
- `referentie/` — oefeningenbibliotheek en recepten.

## Beginnen

1. `/training` — doe je eerste sessie A.
2. Weeg je 2-3× per week 's ochtends en log het even.
3. Doe zondagavond `/weekcheck`.

Dat is alles. 2 sessies per week = een geslaagde week.
