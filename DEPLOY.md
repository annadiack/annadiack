# Portfolio veröffentlichen (GitHub Pages)

Alles Nötige liegt in `portfolio-site.zip` (~41 MB):
- `index.html` — die Website
- `assets/Anna_Diack_CV.pdf` — dein CV zum Download
- `assets/qr-code.png` — QR-Code, der auf https://annadiack.github.io zeigt
- `demos/property/`, `demos/sony/`, `demos/aeris/`, `demos/aurelis/` — die 4 eingebetteten Referenz-Websites (jeweils eigenständig lauffähig, in `index.html` als scrollbare Live-Vorschau eingebettet und einzeln per "Open fullscreen" aufrufbar)

## Schritte

1. `portfolio-site.zip` entpacken.
2. Auf GitHub ein neues Repository erstellen, das **exakt** `annadiack.github.io` heißt (öffentlich, ohne README).
3. Im entpackten Ordner:

```bash
git init
git add .
git commit -m "Portfolio Website"
git branch -M main
git remote add origin https://github.com/annadiack/annadiack.github.io.git
git push -u origin main
```

4. Nach 1–2 Minuten ist die Seite live unter: **https://annadiack.github.io**
5. Falls unter Repo → Settings → Pages nicht automatisch "Deployed", dort als Source `main` / `root` einstellen.

**Wichtig:** Der Ordner ist mit ~41 MB (v.a. die 4 Demo-Seiten) für einen normalen Git-Push völlig unproblematisch — GitHub erlaubt bis 1 GB pro Repo, das hier ist weit darunter.

## QR-Code

`assets/qr-code.png` zeigt bereits auf `https://annadiack.github.io` — statisch, ändert sich nie, direkt druckbar auf CV, LinkedIn-Banner oder Visitenkarte.

## Die 4 eingebetteten Demos

- **Property** — Scroll-Cinematic Immobilien-Website (Frame-Sequenz)
- **Sony WH-1000XM6** — Scrollytelling-Produktseite (Frame-Sequenz)
- **Aeris** — 3D-Studio-Landingpage (aus deinem Next.js/React-Three-Fiber-Projekt als statische Seite exportiert, Assets liegen unter `demos/aeris/_next/`)
- **Aurelis Parfum** — Editorial-Markenwebsite mit eingebettetem Video

Alle vier sind auf der Hauptseite unter "Demos" per Scroll-iframe eingebettet (Lazy-Loading: laden erst, wenn man dorthin scrollt) und zusätzlich per "Open fullscreen"-Link einzeln aufrufbar.

## Hinweise zu Inhalten

- Telefonnummer und Referenzen aus deinem CV habe ich **nicht** auf der öffentlichen Seite gezeigt (Spam-/Datenschutz-Schutz) — nur im CV-PDF-Download enthalten. Sag Bescheid, falls du das anders willst.
- Sprache der Seite: Englisch (passend zu deinem CV/internationalen Profil). Auf Wunsch mache ich eine deutsche Version.
- ASPIRE/REST-API/Digitalisierungsprojekt sind ohne Link markiert (unternehmensintern) — nur das BRCA1-Projekt verlinkt direkt zu deinem GitHub-Repo.
- Bild-Frames von Property & Sony wurden komprimiert (33MB→16MB, 17MB→12MB) für schnelleres Laden, ohne sichtbaren Qualitätsverlust.
