# Høringsanalyse ME/CFS-retningslinjen 2026

Strukturert analyse av alle 458 høringsinnspill levert til Helsedirektoratets utkast til ny nasjonal faglig retningslinje for langvarig utmattelse inkludert ME/CFS.

[![Lisens: CC BY-NC 4.0](https://img.shields.io/badge/Lisens-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

## Om analysen

- **Saksnummer:** Helsedirektoratet 24/13487
- **Høringsutkast publisert:** 4. februar 2026
- **Høringsfrist:** 4. mai 2026
- **Analyse ferdigstilt:** 13. mai 2026
- **Datagrunnlag:** Alle 458 høringsinnspill, ~1 600 sider tekst, 7 formelle dissenser

Analysen er gjennomført rent deskriptivt — den beskriver hva som er sagt i materialet, ikke hvilke argumenter som er saklig sterkest. Alle innspill er behandlet likt etter en konsistent kodebok, uavhengig av lengde, avsendertype eller faglig posisjon.

## Innhold

```
.
├── index.html              # Forside med oversikt og navigasjon
├── dashboard.html          # Interaktivt dashboard (10 tematiske faner)
├── vercel.json             # Vercel-konfigurasjon (CORS, content-types)
├── LICENSE                 # CC BY-NC 4.0
├── README.md               # Denne filen
└── data/
    ├── LESMEG.md           # Detaljert bruksveiledning for datasettet
    ├── kodebok.md          # Den fulle kodeboken (versjon 1.0)
    ├── alle_kodinger.json  # Alle 458 individuelle kodinger
    ├── alle_kodinger.csv   # Flat tabellversjon for Excel
    ├── aktorprofiler.json  # 21 aktørprofiler strukturert
    └── dissenser.json      # Fulltekst av alle 7 dissenser
```

## Dashboard — 10 faner

1. **Forside** — Sentrale tall, omfang av gjennomgangen
2. **Bakgrunn og prosess** — Utkastet, arbeidsgruppe, tidslinje
3. **Dissenser** — Innholdsanalyse av alle syv dissenser
4. **Posisjoner** — De sju hovedposisjonene forklart
5. **Konfliktlinjer** — Sju tematiske skillelinjer
6. **Aktørprofiler** — 21 sentrale aktører i seks kategorier
7. **Oppropet** — Kollektivaksjonen med 3 034 underskrifter
8. **Strukturelle funn** — Standardmal-distribusjon, dissens-asymmetri
9. **Innspilloversikt** — Filtrerbar tabell over alle 458 innspill
10. **Metode og åpenhet** — Kodebok, eksempel-koding, datafiler

## Deployment

### Steg 1: Push til Github

```bash
# Initialiser git i mappen
cd horingsanalyse-mecfs-2026
git init
git add .
git commit -m "Initial publisering av høringsanalysen"

# Koble til Github
git branch -M main
git remote add origin https://github.com/<brukernavn>/horingsanalyse-mecfs-2026.git
git push -u origin main
```

### Steg 2: Koble Vercel til Github

1. Logg inn på [vercel.com](https://vercel.com)
2. Klikk **«Add New...» → «Project»**
3. Velg Github-repoet `horingsanalyse-mecfs-2026`
4. La alle innstillinger stå som default (statiske filer, ingen build-prosess nødvendig)
5. Klikk **«Deploy»**

Vercel oppdager automatisk `vercel.json` og bruker konfigurasjonen.

### Steg 3: Tildelt URL

Etter første deploy får prosjektet en URL i formatet:
- `horingsanalyse-mecfs-2026.vercel.app`

Du kan også koble et eget domene (f.eks. `horing-mecfs-analyse.no`) via Vercel-innstillingene.

### Automatisk redeploy

Etter at Vercel er koblet til Github-repoet:
- Hver push til `main`-grenen utløser automatisk en ny produksjons-deploy
- Hver pull request får sin egen preview-URL

## URL-er etter deployment

| URL | Innhold |
|---|---|
| `/` | Forside med oversikt og lenker |
| `/dashboard.html` | Interaktivt dashboard |
| `/data/kodebok.md` | Kodeboken |
| `/data/alle_kodinger.json` | Alle 458 kodinger som JSON |
| `/data/alle_kodinger.csv` | CSV-versjon for Excel |
| `/data/aktorprofiler.json` | 21 aktørprofiler |
| `/data/dissenser.json` | Fulltekst av alle 7 dissenser |

`vercel.json` setter riktige content-types og CORS-headere så datafilene kan brukes av andre verktøy programmatisk.

## Lokal test før push

Du kan teste pakken lokalt uten Vercel/Github:

```bash
# Python (innebygd HTTP-server)
cd horingsanalyse-mecfs-2026
python3 -m http.server 8000

# Eller med Node.js
npx serve .
```

Deretter åpne `http://localhost:8000/` i nettleseren.

## Forhold til AGREE II-siden

Denne analysen er separat fra `horing.vercel.app`, som er forfatterens egen AGREE II-baserte metodiske vurdering av høringsutkastet (sendt inn som høringsinnspill 2 av 3). De to sidene har ulike formål:

- **`horing.vercel.app`** — Forfatterens eget innspill nr. 2 (AGREE II-skåring som høringssvar)
- **Denne analysen** — Deskriptiv kartlegging av samtlige 458 høringsinnspill

## Lisens

Datasettet er lisensiert under [Creative Commons Attribution-NonCommercial 4.0 International](https://creativecommons.org/licenses/by-nc/4.0/) (CC BY-NC 4.0).

Du har lov til å bruke, dele og bearbeide materialet for ikke-kommersielle formål, så lenge analysen krediteres som:

> Høringsanalyse ME/CFS-retningslinjen 2026, Halvard Nordang. CC BY-NC 4.0.

Direkte sitater fra Helsedirektoratet og dissensbrevene er offentlig tilgjengelige primærkilder som kan brukes etter alminnelige sitatregler.

## Kontakt

For spørsmål om analysen, datasettet, eller for å rapportere feil — opprett en issue i Github-repoet eller kontakt Halvard Nordang direkte.

## Versjonshistorikk

- **v1.0** (13. mai 2026) — Første publisering. Alle 458 innspill ferdigkodet etter kodebok versjon 1.0.
