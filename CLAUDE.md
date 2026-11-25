# CLAUDE.md

Neon Hustle: ein Endless-Hopper im Neon-Cyberpunk-Look, gebaut als Web-Spiel fürs iPhone.

## Konventionen

- Sprache von Code-Kommentaren, Spieltexten und Doku: **Deutsch**.
- Das ganze Spiel bleibt **eine Datei**: `index.html` (HTML, CSS, JS). Keine Build-Tools, keine externen Bilder oder Sounddateien. Schriften kommen von Google Fonts.
- Grafik: Canvas 2D. Teure Leuchteffekte (`shadowBlur`) nur in einmal gerenderten Sprites (`sprite()`), nie pro Frame.
- Sound: live mit Web Audio im `Sound`-Modul erzeugt.
- PWA: `manifest.webmanifest`, `icons/`, `sw.js`. `index.html` holt der Service Worker immer erst aus dem Netz; kommen neue Dateien in den Offline-Speicher (`CORE`), `CACHE` in `sw.js` hochzählen.
- Farben: Lila, Pink, Blau, Cyan auf fast Schwarz; Gold nur für Beute.
- Der Nutzer lernt programmieren: neue Mechaniken mit verständlichen Kommentaren und gut benannten Stellschrauben (Konstanten) bauen.

## Story

Ton: düster, leiser psychologischer Horror – Unbehagen statt Schockmomente. **Die Wendung der Story (die späten Einträge in `MEMORIES`) nicht verraten** – nicht in Antworten, Commits, PR-Texten oder Doku. Snow soll sie beim Spielen selbst entdecken.

## Testen

Mit dem vorinstallierten Playwright `index.html` headless laden, ein paar Züge per Tastatur spielen, auf `pageerror` prüfen und einen Screenshot ansehen. Für seltene Elemente (Datenkanal, Safehouse, Laster) eine Testkopie erzeugen, in der sie sofort vorkommen, und diese danach löschen.

## Roadmap

Siehe `docs/konzept.md`. Leitregel: Jede neue Mechanik muss eine Entscheidung erzeugen.
