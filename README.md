# Lex — De Kwalificatie-onderzoeker 🇳🇱
### A folder-based AI research partner for Dutch worker-classification law

> **One-glance hook.** Most "research assistants" *summarize*. Lex *investigates* — in a domain where the law is literally moving under your feet right now: enforcement resumed **1 Jan 2025**, the **VBAR** bill is mid-flight (narrowed March 2026, not in force), and the **EU Platform Work Directive** is landing. Keeping someone on the right side of *what is settled, what is in motion, and what is not law yet* is exactly the work a summarizer can't do.
>
> **Hook in één oogopslag.** De meeste "research assistants" *vatten samen*. Lex *onderzoekt* — in een domein waar het recht nú onder je voeten beweegt: handhaving hervat per **1-1-2025**, het **VBAR**-wetsvoorstel onderweg (versmald maart 2026, niet in werking), de **EU-Platformrichtlijn** in aantocht. Iemand op de juiste kant houden van *wat gestold is, wat in beweging is, en wat nog geen recht is* — dát kan een samenvatter niet.

*Drop this folder into a Claude Project. Claude becomes Lex. / Zet deze map in een Claude Project. Claude wordt Lex.*

**English readers:** jump to [🇬🇧 English](#-english). **Nederlandstalig:** ga naar [🇳🇱 Nederlands](#-nederlands).

---

## 🇬🇧 English

### What it covers
One narrow, fast-moving corner of Dutch employment law: **whether a working relationship legally is an employment contract (`arbeidsovereenkomst`, art. 7:610 BW) or genuine self-employment (`zzp`)** — i.e. `schijnzelfstandigheid` (bogus self-employment) — and what follows for tax/premium exposure and contracting practice.

This corner was chosen because the law here is *visibly in motion* — which is where a researcher beats a summarizer. Three moving parts at once:
- **Case law moved:** *X/Gemeente Amsterdam* (HR 2020) killed "party intent" as a classification factor; *Deliveroo* (HR 2023) replaced the old test with an open **gezichtspuntencatalogus** (holistic weighing, no single factor decisive).
- **Enforcement moved:** the Tax Authority's `handhavingsmoratorium` ended **1 January 2025** — back-assessments are live again.
- **The statute is moving:** the **VBAR** bill is pending, narrowed in March 2026, **not in force**; the **EU Platform Work Directive** is still being implemented.

### Who it's for
HR/legal advisers, procurement/inhuur managers, in-house counsel, and ZZP'ers weighing their own position. **Most useful work:** pressure-testing a classification *before* someone relies on it — turning "we have a modelovereenkomst, so we're fine" into a sourced, viewpoint-by-viewpoint weighing with the weak spots flagged. It is an **orienting research partner, not a legal or tax opinion.**

### Why it's a *researcher*, not a summarizer
Five behaviours the folder forces (and a summarizer skips):
1. **It interrogates before it answers.** Hand it "is my ZZP'er a problem?" and it asks about your exposure, the lived facts (the gezichtspunten), what you already have, and the period — before any law. (`rules.md` §1)
2. **It weighs sources, and shows which lead.** It makes explicit what is **leading** (statute, Hoge Raad, CJEU = certainty within their reach) versus merely **signalling** (lower-court rulings, blogs, Tax-Authority posture = hints, never certainty). (`reference/bronnenladder.md`)
3. **It refuses to invent citations.** An LLM will hallucinate an ECLI. Lex treats any unverified case as **⚠️ te verifiëren**, and — when the Project has web access — **verifies via the rechtspraak.nl deeplink before citing**. (`rules.md` §3)
4. **It flags coverage gaps & uncertainty.** `rechtspraak.nl` publishes only a *selection*, so "no case found" never means "no law." Every conclusion is labelled *settled / in motion / not yet in force*. (`rules.md` §4, §8)
5. **It keeps a research-ledger.** What I know · what I don't · what would flip the conclusion. (`rules.md` §6)

If its output reads like a Wikipedia paragraph on art. 7:610 BW, it has failed.

### The folder
```
CLAUDE.md          ← entry point: makes Claude become Lex + which files to read, in order
README.md          ← how to use it (NL + EN)
identity.md        ← who Lex is + exact scope
rules.md           ← HOW it researches (the investigative core)
examples.md        ← what good looks like (researcher vs summarizer transcripts)
reference/
  bronnenladder.md            ← source-credibility ladder: leading vs signalling
  vindplaatsen.md             ← where to find/verify (free vs paywalled, ECLI deeplinks, fetch-and-verify)
  kernbegrippen.md            ← key concepts (gezichtspunten, gezag, inbedding, rechtsvermoeden)
  kernarresten-en-wetgeving.md ← the VERIFIED factual spine (rulings + statute + bill status, dated)
```
Each file does one job — folders as architecture, interpretable context. Keep `kernarresten-en-wetgeving.md` current; this domain dates fast.

### How to use it
1. Create a Claude Project, upload all files (keep `reference/`).
2. Bring your real situation; don't over-explain — Lex will ask what it needs.
3. A good first prompt: *"I'm an HR adviser. We've used the same freelance developer 36 hrs/week for 2.5 years on our core product team. Should I worry after 1-1-2025? Here's our contract: [paste]."* Watch what it does *before* it answers.

### Honest limitations
Not advice · no live legal-database connector out of the box (works from what you paste + free public sources + verifiable training knowledge) · authoritative annotations (JAR, NJ, TRA) are paywalled — it flags they exist · the verified spine was checked **2026-05-27**; VBAR and the Platform Directive are moving targets — re-verify.

---

## 🇳🇱 Nederlands

### Wat het dekt
Eén smalle, snel bewegende hoek van het Nederlandse arbeidsrecht: **of een arbeidsrelatie juridisch een arbeidsovereenkomst is (`arbeidsovereenkomst`, art. 7:610 BW) of echt zelfstandig ondernemerschap (`zzp`)** — oftewel `schijnzelfstandigheid` — en wat daaruit volgt voor blootstelling aan loonheffingen/premies en de inhuurpraktijk.

Deze hoek is gekozen omdat het recht hier *zichtbaar in beweging* is — precies waar een onderzoeker een samenvatter verslaat. Drie bewegende delen tegelijk:
- **De rechtspraak bewoog:** *X/Gemeente Amsterdam* (HR 2020) doodde "partijbedoeling" als kwalificatiefactor; *Deliveroo* (HR 2023) verving de oude toets door een open **gezichtspuntencatalogus** (holistische weging, geen factor beslissend).
- **De handhaving bewoog:** het `handhavingsmoratorium` van de Belastingdienst verviel per **1 januari 2025** — naheffingen lopen weer.
- **De wet beweegt:** het **VBAR**-wetsvoorstel is in behandeling, in maart 2026 versmald, **niet in werking**; de **EU-Platformrichtlijn** wordt nog geïmplementeerd.

### Voor wie
HR/juridische adviseurs, inkoop-/inhuurmanagers, bedrijfsjuristen en zzp'ers die hun eigen positie wegen. **Meest nuttige werk:** een kwalificatie stresstesten *vóór* iemand erop vertrouwt — "we hebben een modelovereenkomst, dus we zijn safe" omzetten in een gebronde, gezichtspunt-voor-gezichtspunt-weging met de zwakke plekken benoemd. Het is een **oriënterende onderzoekspartner, geen juridisch of fiscaal advies.**

### Waarom een *onderzoeker*, geen samenvatter
Vijf gedragingen die de map afdwingt (en een samenvatter overslaat):
1. **Het ondervraagt vóór het antwoordt.** Geef het "is mijn zzp'er een probleem?" en het vraagt naar je blootstelling, de geleefde feiten (de gezichtspunten), wat je al hebt, en de periode — vóór enige wet. (`rules.md` §1)
2. **Het weegt bronnen en toont wat leidend is.** Het maakt expliciet wat **leidend** is (wet, Hoge Raad, HvJ EU = zekerheid binnen hun bereik) versus slechts **signalerend** (lagere rechtspraak, blogs, Belastingdienst-posture = hints, nooit zekerheid). (`reference/bronnenladder.md`)
3. **Het weigert citaten te verzinnen.** Een LLM hallucineert een ECLI. Lex behandelt elke ongeverifieerde uitspraak als **⚠️ te verifiëren** en — als de Project web-toegang heeft — **verifieert via de rechtspraak.nl-deeplink vóór het citeert**. (`rules.md` §3)
4. **Het flagt dekkings-gaten & onzekerheid.** `rechtspraak.nl` publiceert maar een *selectie*, dus "geen zaak gevonden" betekent nooit "geen recht". Elke conclusie krijgt het label *gestold / in beweging / nog niet geldend*. (`rules.md` §4, §8)
5. **Het houdt een research-ledger bij.** Wat ik weet · wat ik niet weet · wat de conclusie zou kantelen. (`rules.md` §6)

Leest de output als een Wikipedia-alinea over art. 7:610 BW, dan is het mislukt.

### De map
Zie het schema hierboven (Engelse sectie). Elk bestand doet één taak — mappen als architectuur, interpreteerbare context. Houd `kernarresten-en-wetgeving.md` actueel; dit domein veroudert snel.

### Hoe te gebruiken
1. Maak een Claude Project, upload alle bestanden (houd `reference/`).
2. Breng je echte situatie; leg niet te veel uit — Lex vraagt wat het nodig heeft.
3. Een goede eerste prompt: *"Ik ben HR-adviseur. We huren al 2,5 jaar dezelfde developer 36 u/week in op ons kern-productteam. Moet ik me zorgen maken na 1-1-2025? Hier is ons contract: [plak]."* Let op wat het doet *vóór* het antwoordt.

### Eerlijke beperkingen
Geen advies · standaard geen live juridische-database-koppeling (werkt vanaf wat je plakt + gratis publieke bronnen + verifieerbare trainingskennis) · gezaghebbende annotaties (JAR, NJ, TRA) zitten achter paywall — het flagt dát ze bestaan · de geverifieerde ruggengraat is gecheckt op **2026-05-27**; VBAR en de Platformrichtlijn bewegen — herverifieer.

---

*Built for Weekly Comp #6 — The Researcher. Interpretable-context methodology: each file does one job well. / Gebouwd voor Weekly Comp #6 — The Researcher.*
