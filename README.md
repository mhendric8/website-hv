# Hendricks Ventures — Website

Statischer One-Pager für [hendricks-ventures.com](https://hendricks-ventures.com).
Digitale Services, Programmierung & Beratung.

## Inhalt

| Datei | Beschreibung |
|-------|--------------|
| `index.html` | Landing-Page (Hero, Leistungen, Portfolio, Kontakt, Impressum im Footer) |
| `datenschutz.html` | Datenschutzerklärung (verlinkt aus dem Footer) |
| `assets/` | Bilder (Portfolio-Screenshots) |
| `CNAME` | Custom Domain für GitHub Pages |
| `.nojekyll` | Deaktiviert Jekyll-Processing auf GitHub Pages |

Keine Build-Tools, keine Abhängigkeiten — reines HTML/CSS.

## Lokal ansehen

Einfach `index.html` im Browser öffnen, oder:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Auf GitHub Pages veröffentlichen

```bash
git init
git add .
git commit -m "Initial commit: Hendricks Ventures website"
git branch -M main
git remote add origin git@github.com:<user>/<repo>.git
git push -u origin main
```

Anschließend in den Repo-Einstellungen: **Settings → Pages → Source: `main` / root**.
Die Datei `CNAME` verbindet die Domain `hendricks-ventures.com` automatisch — bei deinem
DNS-Anbieter noch die `A`-Records auf die GitHub-Pages-IPs (bzw. `CNAME` auf
`<user>.github.io`) setzen.

## Noch zu ergänzen

- Impressum-Platzhalter in `index.html` (Name, Anschrift, USt-IdNr.)
- Platzhalter in `datenschutz.html` und rechtliche Prüfung vor Veröffentlichung
