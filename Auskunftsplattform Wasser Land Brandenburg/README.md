# Auskunftsplattform Wasser Land Brandenburg (APW)

Hier gibt es die Daten für Bad Belzig und Umgebung von der Auskunftsplattform Wasser Land Brandenburg zu finden. Diese können direkt für Datenimports per Node-RED verwendet werden.

## Datenimport

Dateinamen müssen mit der ID der Messstelle beginnen und kommagetrennt die Geokoordinaten der Messstelle beinhalten.
Nur so kann sichergestellt werden, dass die Geokoordinaten ebenfalls importiert werden, da diese nicht in den Metadaten der Messstelle vorhanden sind.

- ID,Latitude,Longitude.csv
  - Beispiel: 38413430,52.142172,12.563414.csv

Diese können mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Dateien wird automatisch ein Flow in Node-RED für den Import gestartet.

Erwartete CSV-Struktur der Dateien:

- per Semikolon getrennt, mit Headerzeile
- Beispiel: "Datum";"Präfix";"Wasserstand(GOK) [cm u. GOK]";"Hinweise"
