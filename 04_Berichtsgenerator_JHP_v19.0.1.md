# 04 – Berichtsgenerator JHP V19.0.1

## Grundsatz
Der Berichtsgenerator erstellt Word-Berichte nicht frei, sondern ausschließlich auf Basis eines validierten `.dotx`-Templates oder eines zulässigen Fallback-Skeletts.

## Eingaben
- Projektname
- Objekt
- Standort
- Datum
- Prüfer
- Prüfart
- strukturierte Prüfdaten
- Bildzuordnung

## Erzeugungslogik
1. Template prüfen
2. Pflichtfelder belegen
3. Wiederholbereiche (z. B. Geräte) befüllen
4. Bilder in definierte Slots einfügen
5. Bericht auf Plausibilität prüfen
6. Word-Output freigeben

## Muss-Regeln
- fehlende Pflichtfelder = Abbruch
- Template-Mismatch = HOLD oder STOP
- beschädigte Schutzbereiche = STOP

## Ergebnis
Der Berichtsgenerator liefert einen strukturierten Word-Bericht, der mit Excel/PDF/ZIP konsistent sein muss.
