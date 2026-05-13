# Datasett — Høringsanalyse ME/CFS-retningslinjen 2026

Denne mappen inneholder alle maskinlesbare data fra analysen.

## Filoversikt

### kodebok.md (10 KB)
Den fulle kodeboken (versjon 1.0) som er brukt på alle 458 innspill. Beskriver:
- Sju hovedposisjoner (A_klar, A_modifisert, pragmatisk, tjenestefaglig, B_klar, B_modifisert, uklar)
- Syv konfliktlinjer (felles_vs_egen, canadakriteriene, pem, aktivitet, biopsykososial, tillitsskapende, dissens_støtte)
- 35 argument-tagger
- Kvalitetsmarkører og merknader

### alle_kodinger.json (1,2 MB)
Komplett JSON-fil med alle 458 individuelle kodinger.

Struktur:
```json
{
  "meta": {
    "beskrivelse": "...",
    "saksnummer": "24/13487",
    "antall_innspill": 458,
    "kodebok_versjon": "1.0"
  },
  "kodinger": [
    {
      "id": 1,
      "navn": "...",
      "avsendertype": "...",
      "hovedposisjon": "A_klar",
      "posisjon_per_anbefaling": {...},
      "konfliktlinjer": {...},
      "argumenter": [...],
      "hovedbudskap": "...",
      "sentrale_sitater": [...],
      "kvalitet": "sikker",
      "merknader": "..."
    },
    ...
  ]
}
```

### alle_kodinger.csv (400 KB)
Flat tabellversjon (semikolon-separert) for Excel og statistikkverktøy. 19 kolonner per rad:

| Kolonne | Beskrivelse |
|---|---|
| id | Innspillets løpenummer hos Helsedirektoratet |
| navn | Avsender (privatpersoner anonymisert av Helsedirektoratet) |
| avsendertype | Privatperson, organisasjon, helseforetak osv. |
| pulje | Innleveringspulje 1–5 |
| er_dissens | True/False — markerer formell dissens |
| hovedposisjon | Én av sju kategorier |
| konfliktlinje_* | Sju konfliktlinje-kolonner |
| antall_argumenter | Antall argument-tagger |
| argumenter | Tagger separert med semikolon |
| hovedbudskap | Kortet til 500 tegn |
| antall_sitater | Antall sentrale sitater |
| kvalitet | sikker / delvis_sikker / usikker |
| merknader | Kortet til 300 tegn |

### aktorprofiler.json (30 KB)
De 21 aktørprofilene som strukturert JSON. Inkluderer kjernebudskap, sentrale sitater, koblinger til andre aktører og strukturell betydning for hver av:

**A. Sentrale aktører på den biomedisinske siden (6):**
1. Norges ME-forening
2. ME-foreldrene
3. ME-forskningsgruppen ved Haukeland universitetssykehus og UiB
4. Røysumtunet
5. Pårørendealliansen
6. Norsk Covidforening

**B. Den biopsykososiale tilnærmingen og Nasjonal kompetansetjeneste (3):**
7. Karlsonpsykologene
8. Recovery Norge
9. Nasjonal kompetansetjeneste for CFS/ME

**C. Statlige og regulerende aktører (2):**
10. Folkehelseinstituttet
11. Arbeids- og velferdsdirektoratet (NAV)

**D. Forskning og dokumentasjon (3):**
12. Forskningsstiftelsen Fafo (Anne Kielland)
13. Bjørn Getz Wold (ME-Fondet)
14. Frøydis Lilledalen med flere

**E. Spesielle individuelle aktører (3):**
15. Anonym britisk senior pediater
16. Anonym psykologspesialist med biomedisinsk linje
17. Profesjonsforeningene (samlet)

**F. Refererte aktører som ikke har levert eget innspill (4):**
18. Nina E. Steinkopf (melivet.com)
19. Vegard Bruun Wyller
20. Karolinska Institutet (utmattningssyndrom-modellen)
21. Det øvrige refererte overbelastnings-økosystemet

### dissenser.json (26 KB)
Fulltekst av alle syv formelle dissenser:

**Fag-dissenser i selve høringsutkastet (4):**
1. Tom Farmen Nerli (rehabilitering, Sykehuset Vestfold) — 26.01.2026
2. Linn Breen Herner (psykolog, Oslo universitetssykehus) — 27.01.2026
3. Ingjerd Helene Jøssang (allmennlege, Stavanger) — 26.01.2026
4. Peter Prydz (allmennlege, Hammerfest) — 27.01.2026

**Brukerorganisasjons-dissenser levert som høringsinnspill (3):**
5. Norges ME-forening (Trude Schei) — 26.02.2026
6. Norsk Covidforening (Carina Mørch-Storstein) — 03.03.2026
7. ME-foreldrene (Tanja Thorsen) — april 2026

## Bruksveiledning

### For forskere
JSON-filene er strukturerte for direkte analyse i Python (pandas), R, eller andre statistikkverktøy.

```python
import pandas as pd
df = pd.read_csv('alle_kodinger.csv', sep=';')
print(df['hovedposisjon'].value_counts())
```

### For journalister
CSV-filen kan åpnes direkte i Excel. Bruk filterfunksjonen for å se delgrupper, og kombiner med dashboardet for visuell oversikt.

### For beslutningstakere
Kombiner dashboardets aktørprofiler og dissens-fane med datasettets råmateriale for å spore hvilke argumenter som faktisk forekommer i hvilke deler av materialet.

## Lisens

Fritt tilgjengelig for ikke-kommersielt bruk. Krediter: **«Høringsanalyse ME/CFS-retningslinjen 2026, Halvard Nordang»**.

## Versjon

- **Versjon:** 1.0
- **Generert:** 13. mai 2026
- **Kodebok:** versjon 1.0
- **Datakilde:** Helsedirektoratets høringsside, alle fem innleveringspuljer
