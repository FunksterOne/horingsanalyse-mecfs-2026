# Kvikkstart — fra ZIP til deployet på Vercel på 5 minutter

## 1. Pakk ut og test lokalt (valgfritt, men anbefalt)

```bash
unzip horingsanalyse-mecfs-2026.zip
cd horingsanalyse-mecfs-2026
python3 -m http.server 8000
```

Åpne `http://localhost:8000/` for å verifisere at alt fungerer.

## 2. Lag Github-repo

På Github:
1. Gå til [github.com/new](https://github.com/new)
2. Navn: `horingsanalyse-mecfs-2026`
3. Velg «Public» (eller «Private» hvis du vil)
4. **IKKE** initialiser med README, .gitignore eller lisens (vi har dem allerede)
5. Klikk «Create repository»

## 3. Push lokalt repo til Github

I terminalen, i `horingsanalyse-mecfs-2026`-mappen:

```bash
git init
git add .
git commit -m "Initial publisering av høringsanalysen"
git branch -M main
git remote add origin https://github.com/<DITT-BRUKERNAVN>/horingsanalyse-mecfs-2026.git
git push -u origin main
```

Erstatt `<DITT-BRUKERNAVN>` med ditt Github-brukernavn.

## 4. Koble til Vercel

På Vercel:
1. Gå til [vercel.com/new](https://vercel.com/new)
2. Velg «Import Git Repository»
3. Velg `horingsanalyse-mecfs-2026` fra listen
4. La alle innstillinger stå som default:
   - Framework Preset: «Other»
   - Root Directory: `./`
   - Build Command: (tomt)
   - Output Directory: (tomt)
5. Klikk «Deploy»

Vercel deployer på under et minutt. Resulterende URL:
`https://horingsanalyse-mecfs-2026.vercel.app`

## 5. (Valgfritt) Tilpass URL

Hvis du vil ha en kortere/penere URL:
- I Vercel: Settings → Domains → Edit
- For eksempel `horingsanalyse.vercel.app` eller eget domene

## Etterpå

Hver gang du gjør endringer:
```bash
git add .
git commit -m "Beskrivelse av endring"
git push
```

Vercel deployer automatisk på hver push til `main`-grenen.
