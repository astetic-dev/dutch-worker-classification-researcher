# Demo-draaiboek — bruikbaar script om de demo te reproduceren

Dit is het **bruikbare script**: de exacte prompts die je in een Claude Project plakt (met deze map geüpload) om de demo live te spelen of op te nemen. Per stap staat wat je moet zien en waarop je inzoomt voor de video. De uitgeschreven verwachte uitkomst staat in `voorbeeld-it-contractor-uitgewerkt.md`.

## Vooraf (eenmalig)
1. Maak een nieuw **Claude Project**.
2. Upload **alle** bestanden uit deze map, inclusief `reference/` (níét nodig: de `demo/`-map zelf).
3. Optioneel maar sterk voor de opname: zet **web/fetch aan** in het Project, zodat Lex de citatie live kan verifiëren (toont de fetch-en-verifieer-discipline).
4. Start een nieuwe chat. Plak de prompts hieronder één voor één.

---

## Stap 1 — De openingsprompt (de "val")

**Plak:**
```
We huren al ruim 3 jaar dezelfde developer in via zijn eigen BV. Hij factureert keurig met btw en heeft een KvK-inschrijving. Sinds die handhaving van de Belastingdienst per 2025 vraagt onze controller zich af of we risico lopen — maar het is toch gewoon een zzp'er? Kun je dat bevestigen en even de wet hierop samenvatten?
```
**🎬 Wat je moet zien (en filmen):** Lex vat **niet** samen. Hij weigert de abstracte samenvatting, daagt de framing uit (btw/KvK/"al 3 jaar" dragen niet wat je denkt), en stelt 3–4 gerichte vragen. → Dit is dé "researcher, geen summarizer"-shot. Zoom in op de wedervraag en op de regel over het handhavingsmoratorium (1-1-2025).

## Stap 2 — De antwoorden (maak het een grensgeval)

**Plak:**
```
1. Wij zijn de opdrachtgever; de controller vreest naheffing loonheffingen, en herkwalificatie willen we ook niet.
2. Hij zit vast in één scrumteam op ons hoofdproduct, doet dezelfde stand-ups en sprintplanning als de vaste devs, werkt in onze Jira en repo's.
3. Hij factureert via zijn eigen BV, €95/uur. Daarnaast nog twee andere klanten, samen zo'n dag per maand. Eigen laptop, geen loondoorbetaling bij ziekte, eigen AOV, af en toe acquisitie. Specialist in een framework dat wij zelf niet in huis hebben.
4. Contract staat vervanging toe; één keer een collega uit zijn BV gestuurd toen hij twee weken weg was. Verder doet hij het werk zelf en pakt taken op zoals het team. 36 uur per week.
5. Vooral het risico vanaf nu.
```
**🎬 Wat je moet zien:** Lex weegt de **gezichtspunten** in een naar/weg-tabel (geen afvinkscore), benoemt de **spanning**, en toont expliciet de **LEIDEND**- vs **SIGNALEREND**-regel en het **research-ledger** (wat weet ik / niet / wat kantelt). Eindigt met een eerlijke, gekalibreerde inschatting ("leunt naar arbeidsovereenkomst, maar echt grensgeval") — geen schijnzekerheid. → Zoom in op de tabel + de leidend/signalerend-labels.

## Stap 3 — De bruikbare uitkomst

**Plak:**
```
Ja, graag — geef me de vragen voor onze fiscalist.
```
**🎬 Wat je moet zien:** Lex levert een scherpe, op het dossier toegesneden **vragen-voor-je-adviseur-lijst** — niet generiek, maar precies de punten die de doorslag geven. → Bewijst dat het oriënterend onderzoek een concrete volgende stap oplevert.

## Stap 4 (optioneel, sterke slot-shot) — De citatie-discipline testen

**Plak:**
```
Geef me de exacte ECLI van het Hoge Raad-arrest over platformbezorgers, en die over een pakketbezorger, met data.
```
**🎬 Wat je moet zien:** Lex geeft het **geverifieerde** *Deliveroo*-anker (`ECLI:NL:HR:2023:443`) mét vindplaats, maar **weigert een ECLI te verzinnen** voor de pakketbezorger-zaak die hij niet heeft gecheckt — en biedt de zoekroute/verificatie aan. → Dit is de handtekening-shot: "ik verzin geen recht."

---

## Regie-tips
- **Tempo:** laat elke Lex-reactie even "ademen" in beeld; de kracht zit in dat hij eerst vraagt en eerlijk weegt.
- **Highlights:** gebruik markeringen/zoom op (a) de wedervraag in stap 1, (b) de LEIDEND/SIGNALEREND-regel in stap 2, (c) de weigering in stap 4.
- **Reproduceerbaarheid:** exacte output varieert per run (het is een taalmodel). Het *gedrag* — vragen, wegen, bronnen scheiden, niet verzinnen — is wat consistent moet zijn. Draait een run anders, draai opnieuw; pas de prompts niet aan om een uitkomst te forceren.
- **Koppeling met de video:** stap 1 voedt video-segment 0:00–0:20, stap 2 voedt 0:34–1:06, stap 4 voedt 0:52–1:06 (zie `lex-introductievideo-script.md`).
