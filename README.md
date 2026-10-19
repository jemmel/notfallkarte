# Notfallkarte

Notfallkarte für lange Läufe zum Ausfüllen, Drucken und Laminieren, im Scheckkartenformat (85,6 × 54 mm,
Folie 60 × 95 mm). Jede Angabe lässt sich per Auge vom Druck ausnehmen.
Eine einzige Datei, `notfallkarte.html`, ohne Abhängigkeiten. Die Angaben bleiben im Browser.

Online: https://notfallkarte.janemmel.de (Cloudflare Pages, Projekt `notfallkarte-janemmel-de`)

```powershell
./deploy.ps1 -DryRun   # _site/ bauen (index.html + _headers)
./deploy.ps1           # hochladen; legt beim ersten Mal Projekt, Domain und CNAME an
```

Token wie bei kitaweb: `$env:CLOUDFLARE_API_TOKEN`, `.env` hier oder `../kita/.env`.

Testaufrufe: `?beispiel=1` (Musterdaten), `?stress=1` (lange Texte, alle Häkchen; läuft absichtlich über).
