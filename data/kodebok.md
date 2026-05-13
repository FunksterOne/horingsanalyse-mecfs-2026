# Kodebok for analyse av høringsinnspill – ME/CFS-retningslinjen 2026

**Versjon:** 1.0  
**Bakgrunn:** Utviklet empirisk basert på lesing av 19 innspill (5 pasientorg, 3 HF/RHF, 1 forsknings­gruppe, 2 statlige, 1 profesjonsforening, 1 privat klinikk, 1 kommune, 5 privatpersoner).

---

## Sammendrag av observerte posisjoner

Høringen er polarisert mellom to hovedposisjoner som strukturerer det meste av innspillene:

**Posisjon A – "Separasjonslinjen" (PEM-fokusert, biomedisinsk-ankret):**
- Pasientorganisasjonene (ME-foreldrene, ME-foreningen, Norsk Covidforening, regionlag)
- ME-forskningsgruppen Haukeland/UiB
- Flertallet av enkeltprivatpersoner som har uttalt seg
- Krav: ME/CFS som distinkt klinisk tilstand (G93.3) – atskilt fra "langvarig utmattelse"; PEM som styrende prinsipp; aktivitetsavpasning ("pacing") og føre-var; NICE 2021 som referansegrunnlag

**Posisjon B – "Felles retningslinje" (rehabilitering- og funksjons-orientert):**
- FHI
- Arbeids- og velferdsdirektoratet (NAV)
- Recovery Norge
- Karlsonspsykologene (med egen OKU-teori)
- Helse Fonna HF
- Krav: Felles retningslinje for hele utmattelses-feltet; biopsykososial modell; nevroplastisitet og forklaringsmodeller; vektlegging av at bedring/tilfriskning er mulig; advarsel mot nocebo-effekter

**Posisjon C – "Pragmatisk mellomposisjon":**
- Akershus universitetssykehus, Norsk Fysioterapeutforbund, Norsk Kiropraktorforening, mange HF
- I hovedsak støttende, men ber om presiseringer på begge sider

Recovery Norge og Karlsonspsykologene står ut som de tydeligste eksponenter for posisjon B blant pasient-/aktør-siden. **De tre dissensene** kommer fra posisjon A-siden (ME-foreningen, ME-foreldrene, Norsk Covidforening).

---

## DEL 1 – Klassifisering per innspill

### 1.1 Hovedposisjon (eksklusivt valg, én verdi per innspill)

| Kode | Betegnelse | Kriterium |
|------|-----------|-----------|
| `A_klar` | Posisjon A (klar) | Krever separat retningslinje for ME/CFS, PEM som styrende, kritisk til biopsykososial modell |
| `A_modifisert` | Posisjon A (modifisert) | Vil ha tydeligere skille i én retningslinje, PEM-sentrisk, men aksepterer felles ramme |
| `B_klar` | Posisjon B (klar) | Støtter felles retningslinje, biopsykososial/nevroplastisk modell, vektlegger bedring |
| `B_modifisert` | Posisjon B (modifisert) | Mest enig i felles tilnærming, men anerkjenner behov for PEM-hensyn |
| `pragmatisk` | Pragmatisk/midt | Tar ikke klar side, foreslår presiseringer på begge sider |
| `tjenestefaglig` | Tjenestefaglig | Innspill om praktisk gjennomføring (samhandling, ressurser) uten klar ideologisk side |
| `uklar` | For uklar / for sparsom tekst til å klassifisere | Sparsom tekst eller blandet/inkonsistent budskap |

### 1.2 Posisjon per anbefaling (per kolonne i Excel)

For hver av de 13 anbefalingene som har en egen Excel-kolonne, kodes:

| Kode | Betegnelse |
|------|-----------|
| `støtter` | Støtter anbefalingen som den står |
| `støtter_med_forbehold` | Støtter intensjon, men foreslår presiseringer/justeringer |
| `kritisk` | Vesentlige innvendinger, vil endre |
| `avviser` | Vil ha anbefalingen fjernet eller fullstendig omskrevet |
| `ikke_berørt` | Ikke kommentert |

### 1.3 Argument-koder (multi-label, kan ha 0–10 per innspill)

| Kode | Betegnelse |
|------|-----------|
| `pem_kjerne` | PEM som kardinalsymptom og styrende prinsipp |
| `pem_definisjon` | Kritikk av/forslag til hvordan PEM defineres og operasjonaliseres |
| `egen_retningslinje` | Krav om egen/separat retningslinje for ME/CFS (G93.3) |
| `skille_me_utmattelse` | Krav om tydeligere skille i felles retningslinje |
| `canadakriteriene_støtte` | Støtter Canadakriteriene som primær diagnostisk standard |
| `canadakriteriene_kritikk` | Kritikk av Canadakriteriene (for snevre, for brede, ikke evidenssterke nok) |
| `andre_diagnosekriterier` | Foreslår IOM/SEID, ICC, ME-ICC, ICD-11 eller andre |
| `biopsykososial_kritikk` | Kritikk av biopsykososial modell som overordnet ramme |
| `biopsykososial_støtte` | Eksplisitt støtte til biopsykososial modell |
| `nevroplastisitet` | Vektlegging av nevroplastisk forklaringsmodell |
| `nice_2021` | Referanse til/krav om alignering med NICE 2021 |
| `aktivitet_pacing` | Vektlegging av aktivitetsavpasning/pacing |
| `aktivitet_gradvis_økning` | Vektlegging av gradvis aktivitetsøkning/GET-variant |
| `kognitiv_terapi_støtte` | Eksplisitt støtte til kognitiv atferdsterapi |
| `kognitiv_terapi_kritikk` | Kritikk av kognitiv atferdsterapi for ME/CFS |
| `lp_støtte` | Eksplisitt støtte til Lightning Process |
| `lp_kritikk` | Eksplisitt kritikk av Lightning Process |
| `alvorlig_syke` | Bekymring for alvorlig/svært alvorlig syke, sengeliggende |
| `barn_og_unge` | Eget fokus på barn og unge med ME/CFS |
| `tvang_pasientvern` | Bekymring for tillitsskapende tiltak som tvang |
| `tvang_nødvendig` | Mener tillitsskapende tiltak/myndighet er nødvendig |
| `psykologisering` | Kritikk av psykologisering av sykdommen |
| `nocebo` | Vektlegging av nocebo-effekt fra negative forventninger/prognoser |
| `tilfriskning_håp` | Vektlegger at tilfriskning er mulig / etterlyser optimistisk perspektiv |
| `dårlig_prognose` | Vektlegger at prognosen ofte er dårlig / kritisk til urealistisk optimisme |
| `kunnskapsgrunnlag_smalt` | Kritikk av at kunnskapsgrunnlaget i retningslinjen er for snevert |
| `kunnskapsgrunnlag_brukererfaring` | Etterlyser større vekt på brukererfaringer |
| `kunnskapsgrunnlag_forskning` | Etterlyser strengere forskningsbasering |
| `nav_arbeidsliv` | NAV/uføretrygd/arbeidsliv-perspektiv |
| `tjenester_samhandling` | Etterlyser bedre samhandling mellom nivåer/tjenester |
| `kompetanseheving` | Krav om kompetanseheving av helsepersonell |
| `implementering_konkret` | Konkrete forslag til implementering |
| `arbeidsgruppe_kritikk` | Kritikk av arbeidsgruppens sammensetning eller arbeid |
| `støtter_dissens` | Eksplisitt støtte til de tre dissensene fra arbeidsgruppen |
| `lp_kommersielt` | Kritikk av at LP/Recovery er kommersielle aktører |

### 1.4 Konfliktlinje-matrise (egen kolonne for hver)

For hver av de 7 hovedkonfliktlinjene, kodes posisjonen:

| # | Konfliktlinje | Verdier |
|---|--------------|---------|
| 1 | Én felles vs. atskilt retningslinje | `felles`, `skille_innen_felles`, `egen_for_me`, `ikke_berørt` |
| 2 | Canadakriteriene som primær | `støtter`, `støtter_med_forbehold`, `kritisk`, `avviser`, `ikke_berørt` |
| 3 | PEM som styrende prinsipp | `kjernen`, `viktig`, `ett_symptom`, `nedtonet`, `ikke_berørt` |
| 4 | Aktivitetsregulering – pacing vs. gradvis økning | `kun_pacing`, `pacing_primært`, `balanse`, `gradvis_økning_primært`, `ikke_berørt` |
| 5 | Kognitiv/biopsykososial tilnærming | `avviser`, `kritisk`, `nøytral`, `støtter`, `aktiv_støtte`, `ikke_berørt` |
| 6 | Tillitsskapende tiltak (vs. tvang) | `pasientvern`, `nyansert`, `nødvendig_støtte`, `ikke_berørt` |
| 7 | Støtter dissensene | `støtter`, `nevner_nøytralt`, `kritisk_til_dissens`, `ikke_berørt` |

---

## DEL 2 – Strukturert utdata per innspill

Hvert kodet innspill får følgende JSON-struktur:

```json
{
  "id": 398,
  "navn": "ME-foreldrene",
  "avsendertype": "Pasient-/brukerorganisasjon",
  
  "hovedposisjon": "A_klar",
  
  "posisjon_per_anbefaling": {
    "bakgrunn_metode": "kritisk",
    "fastlege_helhetlig": "kritisk",
    "helhetlig_kartlegging": "kritisk",
    "fastlege_igangsette": "kritisk",
    "canadakriteriene": "støtter_med_forbehold",
    "aktivitetsregulering": "avviser",
    "tverrfaglig_utredning": "kritisk",
    "virksomhetsleder": "kritisk",
    "kommunen_tillit": "kritisk",
    "fastlege_barn": "kritisk",
    "spesialist_barn": "kritisk",
    "lege_ansvar_barn": "kritisk",
    "helsepersonell_barn": "kritisk"
  },
  
  "konfliktlinjer": {
    "felles_vs_egen": "egen_for_me",
    "canadakriteriene": "støtter_med_forbehold",
    "pem": "kjernen",
    "aktivitet": "kun_pacing",
    "biopsykososial": "avviser",
    "tillitsskapende": "pasientvern",
    "dissens_støtte": "støtter"
  },
  
  "argumenter": ["pem_kjerne", "pem_definisjon", "egen_retningslinje", 
                  "biopsykososial_kritikk", "nice_2021", "aktivitet_pacing",
                  "alvorlig_syke", "barn_og_unge", "psykologisering",
                  "dårlig_prognose", "kunnskapsgrunnlag_smalt"],
  
  "hovedbudskap": "Krever at ME med PEM tas ut av den felles retningslinjen og at retningslinjen forankres i NICE 2021. Hevder at sammenblanding av heterogene utmattelsestilstander gir pasientskade.",
  
  "sentrale_sitater": [
    {"tekst": "Det er et strukturelt tegn på at ME med PEM ikke må inngå som del av en generell retningslinje for langvarig utmattelse.", "kontekst": "Om premisset for retningslinjen"},
    {"tekst": "Aktivitetsavpasning bør angis som grunnprinsipp.", "kontekst": "Om aktivitetsregulering"}
  ],
  
  "kvalitet": "sikker",
  "merknader": "40-siders strukturert innspill med 18 deler. Levert som dissens-organisasjon."
}
```

---

## DEL 3 – Kvalitetskriterier

For hvert innspill markerer jeg `kvalitet`:

- `sikker` – tydelig tekst, klar posisjon, kodebar uten skjønn
- `usikker` – flertydig, blandede signaler, eller motsigende utsagn
- `sparsom` – så lite tekst at klassifisering er svært usikker
- `OCR_støy` – PDF-tekst med betydelig OCR-feil; tolket innhold

---

## DEL 4 – Sitatregler

- Maks 25 ord per sitat
- Maks 3 sitater per innspill
- Sitater må være ordrette (med mindre OCR-feil må normaliseres – da markeres dette)
- For sladdede privatperson-PDF-er: aldri navn i sitat eller kontekst, kun rolle hvis åpenbart fra teksten (f.eks. "psykologspesialist")

---

## Endringer som kan komme

Denne kodeboken er foreløpig. Aktuelle utvidelser ved behov:
- Geografisk dimensjon (Helse Vest, Helse Sør-Øst osv.)
- Tidsdimensjon (bolk 1–5 viser om mobilisering kom sent)
- Identifisering av faglig nettverk (hvem refererer til hvem)
