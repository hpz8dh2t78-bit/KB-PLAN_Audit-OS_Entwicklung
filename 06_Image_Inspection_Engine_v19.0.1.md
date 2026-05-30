# 06 – Image Inspection Engine V19.0.1

## Ziel
Bilder werden deterministisch, robust und sichtbar korrekt in das Berichtssystem eingebunden.

## Bildregeln
- feste Slots oder eindeutig benannte Zielbereiche nutzen
- Reihenfolge nicht dem Zufall überlassen
- Seitenverhältnis möglichst erhalten
- Platzierung sichtbar plausibel halten

## Slot-Beispiele
- BILD_1
- BILD_2
- BILD_3
- GERAET_1_BILD_1

## Fehlerlogik
- fehlendes optionales Bild = Warning / leerer Slot
- fehlendes Pflicht-Nachweisbild = HOLD
- unbrauchbare Bilddaten = HOLD oder STOP je nach Kritikalität

## Prüfziele
- Bild vorhanden
- Bild korrekt zugeordnet
- Bild nicht verzerrt
- keine Überlagerung wichtiger Inhalte
