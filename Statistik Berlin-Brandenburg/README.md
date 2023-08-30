# Statistik Berlin Brandenburg

Unter https://www.statistik-berlin-brandenburg.de/ liegen viele interessante Daten, aber leider wird die Seite gerade überarbeitet und es gibt derzeite keine automatische Daten-Schnittstelle. Daher müssen Daten manuell heruntergeladen und hier als CSV abgelegt werden. Bisher passiert das für die Zeitreihe "Landwirtschaftliche Betriebe in Brandenburg" (siehe https://www.statistik-berlin-brandenburg.de/land-und-forstwirtschaft)

## Datenimport

Der Dateiname muss wie folgt lauten:

- landwirtschaftliche_betriebe_brandenburg.csv

Diese Datei kann mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Datei wird automatisch ein Flow in Node-RED für den Import gestartet.

Erwartete CSV-Struktur der Dateien:

- per Semikolon getrennt, mit Headerzeile
- Beispiel: year;value;
