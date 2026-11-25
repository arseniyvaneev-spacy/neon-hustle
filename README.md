# Neon Hustle

Ein Endless-Hopper im Neon-Cyberpunk-Look fürs iPhone. Du bist Kurier eines Syndikats und springst über Hover-Highways, Datenkanäle und Gassen – je mehr Beute, desto heißer wirst du, und desto härter jagt dich die Polizei.

## Spielen

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
| ⬡ EMP-Schild | fängt einen Treffer ab, holt Drohnen in der Nähe runter |
| ⬡ Zeitlupe | 4 s lang läuft alles außer dir in 40 % Tempo |
| ⬡ Tarnmodus | 6 s unsichtbar für Drohnen, Heat eingefroren |
| ⬡ Magnet | 8 s lang wird Beute von den Nachbarfeldern angezogen |

## Aufbau

Alles steckt in einer einzigen Datei, `index.html`: HTML, CSS und JavaScript, ohne Build-Tools und ohne externe Bilder oder Sounds. Grafik wird auf ein `<canvas>` gezeichnet, Sound mit der Web Audio API live erzeugt.

Mehr zur Idee, zum Stil und zur Roadmap: [`docs/konzept.md`](docs/konzept.md).
