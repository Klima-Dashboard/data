# Auskunftsplattform Wasser Land Brandenburg (APW)

Hier gibt es die Daten für Bad Belzig und Umgebung von der Auskunftsplattform Wasser Land Brandenburg zu finden. Diese können direkt für Datenimports per Node-RED verwendet werden.

## Datenimport

Dateinamen müssen mit der ID der Messstelle beginnen und kommagetrennt die Geokoordinaten der Messstelle beinhalten. 
Nur so kann sichergestellt werden, dass die Geokoordinaten ebenfalls importiert werden, da diese nicht in den Metadaten der Messstelle vorhanden sind.

- ID,Latitude,Longitude.zip
  - Beispiel: 38413430,52.142172,12.563414.zip

Diese können mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Dateien wird automatisch ein Flow in Node-RED für den Import gestartet.

Erwartete Dateien im ZIP-Archiv:

- Messreihe beginnend mit der ID der Messstelle und endend mit "_messreihen.csv"
  - Beispiel: 38413430,Belzig,WegRicht.Hagelberg,OP_messreihen.csv
- Metadaten.csv

Erwartete CSV-Struktur der Dateien im ZIP-Archiv:

- per Semikolon getrennt, mit Headerzeile
- Beispiel Messreihe: "Datum";"Präfix";"Wasserstand(NHN) [mNHN]";"Hinweise"
- Beispiel Metadaten: "Metadatum";"Wert"
