# 02 – Runtime Core V19.0.1

## Verbindliche Runtime-Pipeline
1. Projekt initialisieren
2. Muss-Daten prüfen
3. Basisordner vorschlagen / bestätigen
4. Template-Gate ausführen
5. Datenstruktur harmonisieren
6. Bilder prüfen und zuordnen
7. Word / Excel / PDF erzeugen
8. Ergebnisdateien validieren
9. ZIP-Abschluss erzeugen
10. Status auf ABGESCHLOSSEN oder HOLD/STOP setzen

## Zustandsrahmen
- INIT
- DATEN_OFFEN
- TEMPLATE_PRUEFUNG
- DATEN_VALIDIERT
- OUTPUT_IN_ERSTELLUNG
- OUTPUT_VALIDIERT
- ABSCHLUSS_OFFEN
- ABGESCHLOSSEN
- HOLD
- STOP

## HOLD-Auslöser
- Muss-Daten fehlen, sind aber beschaffbar
- Bildzuordnung unklar
- Template noch nicht vollständig geprüft
- Projektstatus widersprüchlich, aber auflösbar

## STOP-Auslöser
- Kein gültiges Template und keine zulässige Fallback-Freigabe
- Kritische Strukturfehler in Template oder Daten
- Abschluss würde falsche oder unvollständige Dateien erzeugen
- Schutzbereiche wären gefährdet

## Abschlussregel
Ein Projekt ist nur abgeschlossen, wenn alle vorgesehenen Ergebnisdateien vorhanden und plausibel sind.
