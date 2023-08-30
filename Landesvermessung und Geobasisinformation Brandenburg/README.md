# LGB (Landesvermessung und Geobasisinformation Brandenburg)
Die Daten des LGB stehen in unterschiedlichen Formaten zur Verfügung. Für die Zwecke des Klima.Daten-Projekts wird eine GeoJSON-Datei benötigt. Diese kann nicht automatisch bezogen werden, sondern muss unter https://geobroker.geobasis-bb.de/gbss.php?MODE=GetProductInformation&PRODUCTID=45C506E5-3E9D-4DE2-9073-C3DB636CE7CF kostenlos "bestellt" werden.

## Datenimport

Für den Import muss die JSON-Datei aus dem ZIP-Ordner umbenannt werden:

- wka.json

Diese Datei kann mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Datei wird automatisch ein Flow in Node-RED für den Import gestartet.

Die Struktur der JSON-Datei darf sich nicht verändern, andernfalls könnte der Import scheitern.
