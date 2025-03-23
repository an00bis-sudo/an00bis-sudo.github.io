pfadithierstein.ch
===

Webauftritt der Pfadi Thierstein Stein: https://pfadithierstein.ch

# HowTo
## Generell
Nach jeder Änderung wird ein neuer "Build" erstellt, was dazu führt, dass die Änderungen auf der Webseite publiziert werden.
Der Build-Job wird automatisch gestartet und muss erfolgreich durchlaufen, was durch den grünen Haken in der Übersicht erkenntlich ist:
![Screenshot 2025-03-23 at 15-04-06 an00bis-sudo_an00bis-sudo github io jekyll](https://github.com/user-attachments/assets/fd47c46c-fb17-4639-b28e-d3e0954e59c5)

Schlägt ein Build fehl, dann liegt irgendwo ein Fehler vor und die Änderungen werden nicht veröffentlicht.

## Downloads
Alle Download-Dateien sind unter [/assets/downloads](https://github.com/an00bis-sudo/an00bis-sudo.github.io/tree/master/assets/downloads).
Wenn ein Download aktualisiert werden soll (Neues QP oder Jahresprogramm), reicht es die Datei zu ersetzen. Dies ist im Folgekapitel "QP aktualisieren" beschrieben.

### QP aktualisieren
* QP als PDF mit dem Namen "Pfadi_QP.pdf" lokal abspeichern.
* Zu https://github.com/an00bis-sudo/an00bis-sudo.github.io/tree/master/assets/downloads navigieren
* Datei hochladen
  * Dadurch wird das alte QP gleich ersetzt. Die Datei muss also zwingend gleich heissen ("Pfadi_QP.pdf")

### Download hinzufügen
Falls auf der Downloadseite ein neues Dokument hinzugefügt werden soll, kann diese in [/assets/downloads](https://github.com/an00bis-sudo/an00bis-sudo.github.io/tree/master/assets/downloads) hochgeladen werden.
Bitte einen sinnvollen Dateinamen verwenden. Orientiert euch an den bestehenden Dateien.

Anschliessend muss in der Datei [`downloads.md`](https://github.com/an00bis-sudo/an00bis-sudo.github.io/blob/master/downloads.md?plain=1) ein neuer Eintrag erstellt werden.

Hier ein Beispiel wie dies aussehen kann:
```yaml
# Beispieltitel
Beschreibung der Datei. Diese wird auf der Downloadseite dargestellt
### [Download](/assets/downloads/Beispiel.pdf)
```
  * Der Teil `[Download](/assets/downloads/Beispiel.pdf)` erstellt einen Link zu der Datei und muss somit mit eurem Dateinamen übereinstimmen. In diesem Beispiel muss die Datei also "Beispiel.pdf" heissen.

## Leiter
* Leiterinfos befinden sich in der Datei [/_data/members.yml](https://github.com/an00bis-sudo/an00bis-sudo.github.io/blob/master/_data/members.yml)
  * Für jede Leitperson existiert ein Eintrag, welcher folgendermassen aussieht:
    ```yaml
    - name: Django
      full_name: Lars Schürch
      functions:
        - Leiter
      group: Wolfsstufe
    ```
    * Es ist wichtig dass die "Einrückung" im Text beachtet wird. Alles immer mit Leerschläge, keine Tabs. Siehe beispielsweise 2 Leerschläge vor `- Leiter`, da dies Teil von `functions:` ist. Am einfachsten einfach bereits bestehende Einträge kopieren.
* Die Leiterbilder sind im Ordner [/assets/pictures/team](https://github.com/an00bis-sudo/an00bis-sudo.github.io/tree/master/assets/pictures/team)
  * Die Bilder werden anhand dem Dateinamen zugeordnert. Für alle Einträge [/_data/members.yml](https://github.com/an00bis-sudo/an00bis-sudo.github.io/blob/master/_data/members.yml) wird automatisch der Bilderordner nach einem gleichnamigen Bild durchsucht.
    Beispielsweise "kjara.jpg" oder "zirpa.jpg".
  * Falls kein Bild gefunden werden kann, wird auf der Webseite ein Placeholder dargestellt: "Noch kein Bild von XY"

* Als Gruppenbild wird das Bild "leitungsteam.jpg unter [/assets/pictures/team](https://github.com/an00bis-sudo/an00bis-sudo.github.io/tree/master/assets/pictures/team) verwendet.
  Soll ein neues Bild verwendet werden, kann dieses ersetzt werden (Gleiches Prozedere wie bei QP).
