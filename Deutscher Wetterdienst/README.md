# DWD (Deutscher Wetterdienst)

Für die Daten des DWD benötigen für weiterführende Berechnungen historischer Mittelwerte von Niederschlagshöhen und Temperaturen. Dafür können die Mittelwerte hier abgelegt werden.

## Datenimport

Der Dateiname muss wie folgt lauten:

- mittelwerte_historisch.csv

Diese Datei kann mit der Zeit immer wieder überschrieben werden mit neuen Inhalten. Nach Aktualisierung dieser Datei wird automatisch ein Flow in Node-RED die neusten Daten bei Imports verwenden.

Erwartete CSV-Struktur der Datei:

- per Semikolon getrennt, mit Headerzeile
- Beispiel: Bezeichnung;Stations_id;Bezugszeitraum;Datenquelle;Jan.;Feb.;März;Apr.;Mai;Jun.;Jul.;Aug.;Sept.;Okt.;Nov.;Dez.;Jahr
  - wichtig hierbei ist die Bezeichnung vorne, die nur in Jahresangaben veränderlich ist, der Rest muss immer gleich bleiben
    - bei Niederschlagshöhen: MITTEL_...
    - bei Temperaturen: MITTEL_TEMP_...
