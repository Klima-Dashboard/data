# Datenzentrale

Hier können zentral CSV-Daten für das Klima-Dashboard Bad Belzig gesammelt und nachvollziehbar abgelegt und verwaltet werden.

## Daten ändern

Jede:r [Nutzer:in mit Schreibberechtigung](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository) hat die Möglichkeit bestehende [Daten zu bearbeiten](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files).

## Neue Datenquelle anlegen
Neue Datenquellen können von [Nutzer:innen mit Schreibberechtigung](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository) erstellt werden. Es bietet sich dabei an, einen eigenen Ordner und eine separate Readme-Datei zu erstellen. Anschließend muss zunächst ein passender Node-RED-Flow erstellt werden, der die Daten per Post-Request entgegen nimmt. Damit eine Änderung an den Daten dann auch den Import auslöst, können die [Github-Workflows](https://docs.github.com/en/actions/using-workflows) genutzt werden. Eine Mustervorlage liegt hier: https://github.com/Klima-Dashboard/data/blob/main/.github/workflows/import-template.yml


## Aktuelle Datenübersicht
- [Auskunftsplattform Wasser Land Brandenburg (APW)](/Auskunftsplattform%20Wasser%20Land%20Brandenburg)
- [Energieagentur Brandenburg](/Energieagentur%20Brandenburg)
- [Forst Brandenburg](/Forst%20Brandenburg)
- [Landesvermessung und Geobasisinformation Brandenburg (LGB)](/Landesvermessung%20und%20Geobasisinformation%20Brandenburg)
- [Statistik Berlin Brandenburg](/Statistik%20Berlin-Brandenburg)
- [The Things Network](/The%20Things%20Network)
- [openSenseMap](/openSenseMap)
