# 08 – Testfälle V19.0.1

## Ziel
Die Testfälle prüfen, ob V19.0.1 in der Praxis die gewünschte deterministische und robuste Logik einhält.

## Testfall 1 – Saubere Standardvorlage
- gültige `.dotx`
- alle Pflichtfelder vorhanden
- Ergebnis: Berichtserstellung erlaubt

## Testfall 2 – Falscher Dateityp
- Vorlage liegt nur als `.docx` vor
- Ergebnis: STOP

## Testfall 3 – Template-Mismatch
- Prüfart passt nicht zur Vorlage
- Ergebnis: HOLD oder STOP je nach Schwere

## Testfall 4 – Fehlende Pflichtbilder
- Nachweisbilder fehlen bei bildpflichtigem Vorgang
- Ergebnis: HOLD

## Testfall 5 – Abschluss unvollständig
- ZIP ohne PDF oder Excel, obwohl vorgesehen
- Ergebnis: Projekt nicht abgeschlossen

## Testfall 6 – Schutzbereich beschädigt
- Header/Footer würden überschrieben
- Ergebnis: STOP
