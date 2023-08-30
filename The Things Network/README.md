# The Things Network

Hier gibt es die Daten für Bad Belzig von Sensoren des The Things Network zu finden. Diese können direkt für Datenimports per Node-RED verwendet werden.

## Datenimport

Der Dateiname muss wie folgt lauten:

- ttn-sensoren.csv

Diese Datei kann mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Datei wird automatisch ein Flow in Node-RED für den Import gestartet.

Erwartete CSV-Struktur der Dateien:

- per Semikolon getrennt, mit Headerzeile
- Beispiel: device_id;measurement;latitude;longitude
