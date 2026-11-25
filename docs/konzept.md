# Neon Hustle – Konzept

## One-Pager

**Ziel:** Ein Endless-Hopper im Neon-Gangster-Cyberpunk-Look, der auf dem iPhone im Browser läuft (später als App auf dem Home-Bildschirm) – und an dem Snow Spieleprogrammierung lernt.

**Für wen:** Für mich und Freunde; für alle, die Spiele mögen, bei denen eine Runde eine Minute dauert und man sofort noch mal will.

**Kern:** Du bist Kurier eines Syndikats in einer Neon-Megacity und springst Feld für Feld über Hover-Highways, Datenkanäle und Gassen. Beute bringt Punkte und Heat. Mehr Heat bedeutet schnelleren Verkehr und Polizei-Drohnen. Steuerung: Tippen = vorwärts, Wischen = seitlich oder zurück.

**Abbruchkriterium:** Macht eine neue Mechanik keinen Spaß, wenn man sie 5 Runden am Stück spielt, kommt keine Grafik drauf – dann wird erst an der Mechanik gedreht.

**Leitregel:** Jede neue Mechanik muss eine Entscheidung erzeugen (Risiko oder Sicherheit), sonst ist sie nur Lärm.

## Stil

| Element | Umsetzung |
|---|---|
| Farben | fast schwarz-violett, Lila, Pink, Blau, Cyan; Gold nur für Beute |
| Figur | Kurier mit Hoodie, LED-Visier, Goldkette |
| Fahrzeuge | E-Limousinen (Pink, Cyan, Blau), Sattelschlepper (Violett) |
| Stimmung | Neon-Glow, Regen, Scanlines, Stadt-Dunst |
| Schrift | Orbitron (Anzeigen), Rajdhani (Text) |

## Was schon drin ist

- Raster mit 9 Spalten, endlos erzeugte Reihen (Straße, Gasse, Datenkanal, Safehouse, Magnetbahn, Laser-Gitter)
- Beute (◆) und Heat (5 Stufen): schnellerer Verkehr, Polizei-Drohnen mit Vorwarnung
- Combo-Multiplikator (bis ×5) und Near-Miss-Bonus mit Mini-Zeitlupe
- Datenkanal mit treibenden Server-Plattformen, auf denen man mitfährt
- Safehouse: Heat kühlt schnell ab, keine Drohnen, kostet aber die Combo
- Sound und Synthwave-Musik, live mit Web Audio erzeugt; Intensität folgt der Heat
- Events (ab Reihe 12, etwa alle 20–30 s): Blackout, Rush Hour, Razzia
- Power-ups (ab Reihe 8, auf ca. 6 % der Reihen): EMP-Schild, Zeitlupe, Tarnmodus, Magnet
- Daily Run (feste Stadt pro Tag per Seed) mit teilbarem Ergebnis
- Missionen mit Sternen und 6 Rängen
- Signature-Events pro Bezirk (Chance 45 % statt eines allgemeinen Events): Ampel-Hack (Verkehr kriecht), Hafennebel (Sicht nur ~2 Reihen, keine Drohnen), Goldrausch (Beute überall, ×3), Express-Takt (Züge im Dauertakt, Gleis +5), Schwerlast-Konvoi (Verkehr langsamer, Near-Miss ×3)
- Faire Treffer: bis zur Hälfte eines Sprungs zählt das alte Feld; kleinere Trefferzonen (`HIT_PAD`, `CAR_SHRINK`); Drohnen nie über Gassen
- Cosmic Neon-Trip (ab Rang Runner, `TRIP`): schneller, Punkte ×2, Beat-Sprung-Bonus, Stufen alle 25 Reihen, psychedelische Effekte (abschaltbar), eigene Bestenliste
- Story „Die Spiegelkönigin“ (Schneewittchen-Motiv, leiser psychologischer Horror): Der Jäger als Verfolger (`HUNTER`), 16 Erinnerungs-Splitter in 5 Kapiteln (`MEMORIES`, `CHAPTERS`), Funksprüche von SPIEGEL und Eins (`RADIO`), Archiv-Screen
- Bestenliste (lokal): Top 10 für Standard und Daily getrennt, mit Datum und Bezirk
- Garderobe: vier Outfits (Syndikat-Kurier, Neonläufer, Nachtgeist, Pulse-Rider), freigeschaltet bei 0/4/8/12 Sternen; ändern nur die Farben
- Bezirke: Sektor 7, Hafen 9, Neon-Basar, Kuppelstadt, Untergrund, freigeschaltet über den Rang (0–4); eigene Palette und Reihen-Mischung (`DISTRICTS`), Steuerung und Punkte gleich. Der Daily Run spielt immer in Sektor 7.

## Roadmap

1. **Zwei Bezirke über dem höchsten Rang:** Skydeck (schnelle Magnetbahnen, lange Datenkanal-Blöcke) und Spiegelbezirk (gleichmäßiger, sehr dichter Verkehr), je mit eigener Palette, Mischung und Freischaltung.
2. **Abzeichen-Schrank:** eigener Screen mit Kacheln je Bezirk und den erreichten Rängen; gesperrte Kacheln abgedunkelt mit Rang-Anforderung.
3. **Später / nur wenn Zeit:** Outfits mit Beute kaufen, Boss (Polizei-Mech).
4. **Veröffentlichung:** GitHub Pages einschalten (siehe README); App Store nur mit Mac und Developer-Account.

**Nicht vor Version 1:** Shop, Skins, mehrere Charaktere.
