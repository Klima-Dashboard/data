# Energieagentur Brandenburg

Hier gibt es die Daten für Bad Belzig von der Energieagentur Brandenburg zu finden. Diese können direkt für Datenimports per Node-RED verwendet werden.

## Datenimport

CSV-Struktur:

- per Semikolon getrennt, UTF-8, mit Headerzeile
- Beispiel: jahr;schluessel;typ;gemeinde;amt_id;amt;landkreis_id;landkreis;region_id;region;einwohner_gesamt_anzahl;

Dateinamen müssen wie folgt lauten:

- energiesteckbrief_daten_komplett.csv
- strom-_und_waermeerzeugung_ee_komplett__summe.csv
- strom-_und_waermeerzeugung_ee_komplett__zeitreihe_co2__summe.csv

Diese können mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Dateien wird automatisch ein Flow in Node-RED für den Import gestartet.
