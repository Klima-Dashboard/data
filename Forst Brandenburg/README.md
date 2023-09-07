# Forst Brandenburg

Forst Brandenburg gibt einen jährlichen "Waldzustandsbericht" als PDF heraus. Aus diesem wurden manuell Daten zum Waldszustand in ein CSV-Format übertragen. Durch Fortschreibung dieses CSV können die Daten aktualisiert werden.

## Datenimport

Die Dateinamen müssen wie folgt lauten:

- waldzustandsbericht-kronenverlichtung.csv
- waldzustandsbericht-schadstufen.csv

Diese können mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Dateien wird automatisch ein Flow in Node-RED für den Import gestartet.

Erwartete CSV-Struktur der Dateien:

- per Semikolon getrennt, mit Headerzeile
- Beispiel Kronenverlichtung: Jahr;Kronenverlichtung
- Beispiel Schadstufen: Jahr;Baumart;Schadstufe 0;Schadstufe 1;Schadstufe 2-4
