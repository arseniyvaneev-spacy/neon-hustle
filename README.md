# Neon Hustle

Ein Endless-Hopper im Neon-Cyberpunk-Look fürs iPhone. Du bist Kurier eines Syndikats und springst über Hover-Highways, Datenkanäle und Gassen – je mehr Beute, desto heißer wirst du, und desto härter jagt dich die Polizei.

## Spielen

**Als App aufs iPhone (empfohlen):**

1. Auf GitHub: *Settings → Pages → Build and deployment → Source: Deploy from a branch*, Branch `main`, Ordner `/ (root)`, speichern. (Mit kostenlosem Konto muss das Repo dafür öffentlich sein.)
2. Nach etwa einer Minute läuft das Spiel unter `https://arseniyvaneev-spacy.github.io/neon-hustle/`.
3. Die Adresse in **Safari** öffnen → **Teilen** → **„Zum Home-Bildschirm“**. Danach startet Neon Hustle mit eigenem Icon im Vollbild und läuft nach dem ersten Laden auch offline.

**Sonst:**

- **Am Rechner:** `index.html` im Browser öffnen. Steuerung mit den Pfeiltasten, `M` schaltet den Ton.
- **Auf dem iPhone:** Tippen = vorwärts, Wischen = links, rechts oder zurück. Steht der Stummschalter auf lautlos, bleibt das Spiel stumm.

## Mechaniken

| Mechanik | Kurz erklärt |
|---|---|
| ◆ Beute | +3 Punkte (mal Multiplikator), erhöht die Heat |
| Heat | 5 Stufen: schnellerer Verkehr, Polizei-Drohnen, Sirenenlicht, treibendere Musik |
| Combo | ohne Pause vorwärts → Multiplikator bis ×5; nach 1,1 s Stillstand weg |
| Near-Miss | knapp an einem Auto vorbei → Bonus und kurze Zeitlupe |
| Datenkanal | nur auf Server-Plattformen landen, sie tragen dich mit |
| Safehouse | Heat kühlt schnell ab, keine Drohnen – kostet aber die Combo |
| Magnetbahn | Gleis blinkt rot und läutet, dann rast ein langer Zug durch |
| Laser-Gitter | Gassen mit Laser im Takt (flackert vor dem Einschalten); cyan markierte Spalten sind immer frei |
| Blackout | Stadt dunkel, nur Lichtkreis und Scheinwerfer; keine Drohnen, Heat kühlt doppelt |
| Rush Hour | Verkehr 45 % schneller, Beute zählt doppelt |
| Razzia | Heat +2 und Drohnenstaffel; wer überlebt, bekommt Bonus |
| Bezirks-Events | jeder Bezirk hat sein eigenes Event: Ampel-Hack (Sektor 7), Hafennebel (Hafen 9), Goldrausch (Neon-Basar), Express-Takt (Kuppelstadt), Schwerlast-Konvoi (Untergrund) |
| ⬡ EMP-Schild | fängt einen Treffer ab, holt Drohnen in der Nähe runter |
| ⬡ Zeitlupe | 4 s lang läuft alles außer dir in 40 % Tempo |
| ⬡ Tarnmodus | 6 s unsichtbar für Drohnen, Heat eingefroren |
| ⬡ Magnet | 8 s lang wird Beute von den Nachbarfeldern angezogen |

## Cosmic Neon-Trip

Eigener Modus, freigeschaltet ab Rang **Runner**: Verkehr 1,6× so schnell, Punkte doppelt, Musik mit 140 statt 112 BPM. Springst du genau auf den Bass, gibt es **Beat-Bonus** und die Combo hält länger – ein schrumpfender Ring um deine Figur zeigt den Takt. Alle 25 Reihen wird es eine Stufe intensiver (bis Stufe VI). Effekte: Farbrausch, Lichtschweife, Beat-Puls, Warp-Streifen. Im Menü lassen sich die Effekte reduzieren („Trip-Effekte“); bei „Bewegung reduzieren“ am Gerät sind sie von Anfang an aus. Eigene Bestenliste.

## Daily Run und Missionen

- **Daily Run:** Jeden Tag eine feste Stadt, für alle gleich (nach lokalem Datum). Eigener Tagesbestwert und ein Ergebnis zum Kopieren und Teilen.
- **Missionen:** Immer drei aktiv, z. B. „Sammle 10 Beute in einem Run“ oder „Überlebe eine Razzia“. Jede erfüllte Mission bringt einen Stern; alle 4 Sterne steigt dein Rang (Laufbursche → Kurier → Runner → Fixer → Schatten → Syndikats-Boss) und die Ziele werden härter.

- **Bestenliste:** die zehn besten Läufe, Standard und Daily getrennt, mit Datum und Bezirk (Startmenü → „Bestenliste“).
- **Garderobe:** vier Outfits, freigeschaltet bei 0, 4, 8 und 12 Sternen; sie ändern nur die Farben deiner Figur.
- **Bezirke:** Sektor 7, Hafen 9, Neon-Basar, Kuppelstadt und Untergrund, freigeschaltet über deinen Rang. Jeder hat eigene Farben und eine eigene Mischung aus Straßen, Kanälen, Bahnen, Lasern und Safehouses. Der Daily Run läuft immer in Sektor 7.

Fortschritt, Rekorde, Missionen, Outfit und Bezirk werden nur im Browser auf deinem Gerät gespeichert.

## Aufbau

Das Spiel steckt in einer einzigen Datei, `index.html`: HTML, CSS und JavaScript, ohne Build-Tools und ohne externe Bilder oder Sounds. Grafik wird auf ein `<canvas>` gezeichnet, Sound mit der Web Audio API live erzeugt. Dazu kommen `manifest.webmanifest` und `icons/` (App-Name und -Icon) sowie `sw.js` (Service Worker für Offline-Spielen).

Mehr zur Idee, zum Stil und zur Roadmap: [`docs/konzept.md`](docs/konzept.md).
