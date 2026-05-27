# Referentie — Waar je bronnen vindt (`vindplaatsen`)

Hoe en waar je verifieert, zodat de researcher de citatie-discipline kan naleven in plaats van te gokken. Onderscheidt **gratis** van **achter paywall**, en geeft de verificatiepatronen.

## Gratis / publiek (gebruik deze om te verifiëren)

| Bron | URL-patroon | Wat het geeft | Tier |
|------|-------------|---------------|------|
| **Wetten.overheid.nl** | `wetten.overheid.nl` | Officiële geconsolideerde wetgeving met geldigheidsdata. BW Boek 7 (art. 7:610 e.v.), Wet DBA, later VBAR. | 1 (leidend) |
| **Rechtspraak.nl / uitspraken** | `https://uitspraken.rechtspraak.nl/details?id=ECLI:NL:...` | Volledige tekst van *gepubliceerde* uitspraken + metadata, gesleuteld op **ECLI**. Dé manier om een citaat te verifiëren. | 2–5 |
| **Rechtspraak Open Data API** | RESTful service, ECLI-metadata/documenten als XML | Programmatische verificatie; >800k volledige teksten, miljoenen méér als alleen metadata. | 2–5 |
| **EUR-Lex / CURIA** | `eur-lex.europa.eu`, `curia.europa.eu` | EU-richtlijnen (incl. Platformrichtlijn) en HvJ-uitspraken. | 1/3 (leidend) |
| **Tweedekamer.nl** | zoek op wetsvoorstelnummer (VBAR = **36783**) | Live wetgevingsstatus: Kamerstukken, nota's van wijziging, stemmingen. Manier om te checken of VBAR nog loopt/gewijzigd is. | — (status) |
| **Rijksoverheid.nl / Belastingdienst** | `belastingdienst.nl`, `rijksoverheid.nl` | Handhavingshouding, schijnzelfstandigheid-pagina's, beleidsuitleg. | Posture (signalerend) |
| **Advocatenblad — Kroniek Arbeidsrecht** | `magazine.advocatenblad.nl` | Gratis jaarlijks deskundig overzicht; goed om de belangrijke arresten van het jaar te spotten. | 8 → wijst omhoog |

## Achter paywall (weet dát ze bestaan; flag wanneer relevant)

| Bron | Wat het is | Gedrag van de researcher | Tier |
|------|-----------|--------------------------|------|
| **JAR — Jurisprudentie Arbeidsrecht** (SDU/OpMaat) | *De* leidende arbeidsrechtelijke uitsprakenbundel; selecteert de belangrijke HR-arresten (altijd met de A-G-conclusie), plus lagere rechtspraak + HvJ/EHRM, met deskundige annotaties. | Heeft een uitspraak een JAR-annotatie, zeg dat dan en raad hem aan — ook als je hem niet kunt lezen. Sommige kantoren publiceren losse JAR-noten gratis als pdf — gerichte zoekactie waard. | 6 (duidend) |
| **Kluwer InView / Navigator** | Brede juridische database, arbeidsrecht-collectie, geannoteerd. | Benoem het als de plek waar een gebruiker *mét toegang* verder moet zoeken. | 6/7 |
| **NJ, TRA, ArbeidsRecht** | Gezaghebbende tijdschriften/annotaties. | Idem — flag het bestaan, verzin nooit de inhoud. | 6 |

## Het ECLI-verificatiepatroon (kerndiscipline)

Een **ECLI** (European Case Law Identifier) ziet eruit als `ECLI:NL:HR:2023:443`:
- `NL` = land · `HR` = instantie (HR = Hoge Raad; `PHR` = Parket bij de HR, dus de A-G-conclusie; `GHxxx` = gerechtshof; `RBxxx` = rechtbank) · `2023` = jaar · `443` = volgnummer.

**Om elke uitspraak die de researcher noemt te verifiëren:** bouw de deeplink
`https://uitspraken.rechtspraak.nl/details?id=ECLI:NL:HR:2023:443`
en bevestig dat die naar een echte uitspraak leidt waarvan de overweging klopt met de claim.

### Fetch-en-verifieer-workflow (als de Project web-/fetch-toegang heeft)

Heeft de omgeving web- of fetch-toegang, dan **gokt de researcher niet — hij verifieert eerst**:
1. Bepaal de ECLI/vindplaats die je wilt aanhalen.
2. Open de rechtspraak.nl-deeplink (of zoek via wetten.overheid.nl / EUR-Lex) en lees de uitspraak/bepaling.
3. Citeer pas ná bevestiging, en zeg erbij: *"geverifieerd via rechtspraak.nl op [datum]"*.
4. Lukt verifiëren niet (geen toegang, niet vindbaar, dekking-gat) → behandel als **⚠️ te verifiëren** en zeg expliciet dat je het niet hebt kunnen bevestigen.

Heb je géén fetch-toegang, val dan terug op de discipline: lever de **zoekroute** ("zoek op rechtspraak.nl naar *Deliveroo* + Hoge Raad + 2023") in plaats van een nummer dat je mogelijk gehallucineerd hebt.

> De eerlijke default bij een gevraagd citaat dat je niet hebt geverifieerd: geef de zoekroute, niet een nummer uit je hoofd.
