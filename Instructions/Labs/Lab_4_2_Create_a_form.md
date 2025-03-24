---
lab:
  title: 'Lab 4.2: Erstellen von Formularen'
---

# Lab 4.2: Erstellen von Formularen

## Szenario
Das Bellows College ist eine Bildungsorganisation mit mehreren Campusgebäuden. Viele der Lehrer und Administratoren am Bellow College müssen an Veranstaltungen teilnehmen und Artikel kaufen. Historisch gesehen war die Nachverfolgung dieser Ausgaben eine Herausforderung.
Die Campusverwaltung möchte ihr Spesenabrechnungssystem modernisieren, indem den Mitarbeitern eine digitale Möglichkeit zum Melden von Ausgaben an die Hand gegeben wird.
Während dieses Kurses erstellen Sie Anwendungen und führen Automatisierung durch, damit die Mitarbeitenden des Bellows College Ausgaben verwalten können.

## Weiterführende Schritte des Lab
Nach erfolgreichem Abschluss dieses Labs haben Sie Folgendes erreicht:
- Die Anpassung des Tabellenformulars an Ihre Bedürfnisse.

Wir werden mit folgenden Komponenten arbeiten:
- Formulare: Hier erstellt bzw. aktualisiert der Benutzer neue Zeilen in den Tabellen.

## Voraussetzungen
- Beendigung von Modul 1 Lab 0 – Lab-Umgebung überprüfen

## Übung 1: Ansichten und Formulare anpassen
**Ziel**: In dieser Übung passen Sie Ansichten und Formulare der benutzerdefinierten erstellten Tabellen an, die in der modellgesteuerten App verwendet werden.

### Aufgabe Nr. 1: Bearbeiten des Spesenabrechnungsformulars
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen und öffnen Sie die Tabelle „Spesenabrechnung“ aus.
6. Wählen Sie im Abschnitt „Datenfunktionen“ die Option **Formulare** aus, und öffnen Sie das Formular „Informationen“ mit dem Hauptformulartyp. (Wichtig: Stellen Sie sicher, dass Sie das Formular mit dem Formulartyp Main (Haupt) auswählen.)

**WICHTIG**: Da alle Formulare standardmäßig „Information“ heißen, müssen Sie unbedingt überprüfen, ob das von Ihnen ausgewählte Formular den Formulartyp „Haupt“ hat, und keinen anderen. Standardmäßig verfügt das Formular über zwei Felder: „Report Name“ (Berichtname) und „Owner“ (Besitzer).

### Aufgabe Nr. 2: Auswählen von Spalten für das Formular
1. Wählen Sie auf der rechten Seite des Bildschirms im Eigenschaftenfenster das Feld **Name** aus und ändern Sie es in `Report Information`.
2. Wählen Sie **Tabellenspalten** im linken Navigationsbereich aus, und fügen Sie die folgenden Felder unter dem Feld „Owner“ (Besitzer) hinzu, indem Sie Spalten in das Formular ziehen oder einfach auf die Spaltennamen klicken:
    - Beschreibung
    - Berichtszweck
    - Berichtsfälligkeitsdatum
    - Berichtssumme
3. Ziehen Sie die Spalte **Statusgrund**, und legen Sie sie auf der Kopfzeile des Formulars ab. Die Kopfzeile ist der obere rechte Bereich des Formulars. Möglicherweise müssen Sie das Eigenschaftenpanel auf der rechten Seite des Bildschirms zuklappen, um das Feld im Formular anzuzeigen.
4. Ziehen Sie die Spalte **Letztes Datum für die Genehmigung** und legen Sie sie neben dem Statusgrund im Formularkopf ab.
5. Wählen Sie das Feld **Besitzer** aus. Ändern Sie im Eigenschaftenpanel die Bezeichnung in *`Requestor`*.
6. Wählen Sie links im Navigationsbereich die Option **Komponenten** aus.
7. Wählen Sie den 1-spaltigen Abschnitt aus, um ihn unter dem aktuellen Abschnitt hinzuzufügen.
8. Ändern Sie im Eigenschaftenpanel die Bezeichnung **`Expense Lines`**.
9. Wenn der Abschnitt „Spesenzeile“ noch ausgewählt ist, suchen und wählen Sie die Komponente **Subgrid** (Unterraster) aus.
10. Aktivieren Sie das Kontrollkästchen **Verwandte Datensätze anzeigen**.
11. Legen Sie die Tabelle auf **Spesenzeilen (Spesenabrechnung)** fest.
12. Legen Sie die Standardansicht auf **Aktive Spesenzeilen** fest.
13. Wählen Sie **Fertig** aus.
14. Wählen Sie oben rechts **Speichern und Veröffentlichen** aus, und warten Sie, bis der Speicher- und Veröffentlichungsvorgang abgeschlossen ist.
15. Wählen Sie die Schaltfläche „Zurück“ oben links auf dem Bildschirm. Sie sollten sich nun wieder im Formular für die Tabelle Expense Report (Spesenabrechnung) befinden.

### Aufgabe Nr. 3: Bearbeiten eines aktiven Spesenzeilenformulars
In diesem Vorgang ändern wir das Formular, das zum Hinzufügen von Spesenpositionen verwendet wird.

1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option Lösungen aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen und öffnen Sie die Tabelle „Spesenzeile“.
6. Wählen Sie im Abschnitt „Datenfunktionen“ die Option Formulare aus, und öffnen Sie das Formular „Informationen“ mit dem Hauptformulartyp. (Wichtig: Stellen Sie sicher, dass Sie das Formular mit dem Formulartyp Main (Haupt) auswählen.)

**WICHTIG**: Da alle Formulare standardmäßig „Information“ heißen, müssen Sie unbedingt überprüfen, ob das von Ihnen ausgewählte Formular den Formulartyp „Haupt“ hat, und keinen anderen. Standardmäßig verfügt das Formular über zwei Felder: „Spesentitel“ und „Besitzer“.

1. Wählen Sie auf der rechten Seite des Bildschirms im Bereich **Eigenschaften** das Feld **Anzeigename** aus und ändern Sie es in `Item Details`.
2. Wählen Sie **Tabellenspalten** im linken Navigationsbereich aus, und fügen Sie die folgenden Felder unter dem Feld „Owner“ (Besitzer) hinzu, indem Sie Spalten in das Formular ziehen oder einfach auf die Spaltennamen klicken:
    - Spesentyp
    - Item Description
    - Ausgabenbetrag
    - Spesenabrechnung
3. Ziehen Sie die Spalte **Statusgrund**, und legen Sie sie auf der Kopfzeile des Formulars ab. Die Kopfzeile ist der obere rechte Bereich des Formulars. Möglicherweise müssen Sie das Eigenschaftenpanel auf der rechten Seite des Bildschirms zuklappen, um das Feld im Formular anzuzeigen.
4. Wählen Sie die Schaltfläche **Speichern und veröffentlichen** aus.
