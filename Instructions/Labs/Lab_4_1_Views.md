---
lab:
  title: 'Lab 4.1: Visualisieren von Daten mit Ansichten'
---

# Lab 4.1: Visualisieren von Daten mit Ansichten

## Szenario

Das Bellows College ist eine Bildungsorganisation mit mehreren Campusgebäuden. Viele der Lehrer und Administratoren am Bellow College müssen an Veranstaltungen teilnehmen und Artikel kaufen. Historisch gesehen war die Nachverfolgung dieser Ausgaben eine Herausforderung.

Die Campusverwaltung möchte ihr Spesenabrechnungssystem modernisieren, indem den Mitarbeitern eine digitale Möglichkeit zum Melden von Ausgaben an die Hand gegeben wird.

Während dieses Kurses erstellen Sie Anwendungen und führen Automatisierung durch, damit die Mitarbeitenden des Bellows College Ausgaben verwalten können.

## Weiterführende Schritte des Lab

Im Rahmen der Erstellung der modellgesteuerten App führen Sie Folgendes aus:

Erstellen Sie unterschiedliche Ansichten zum Anzeigen von Spesenabrechnungselementen.

Wir werden mit folgenden Komponenten arbeiten:

Ansichten: Mithilfe von Ansichten kann der Benutzer die vorhandenen Daten in Form einer Tabelle anzeigen.

## Voraussetzungen

Abschluss von Modul 1 Lab 0 – Überprüfen der Lab-Umgebung

## Übung 1: Verwalten von Ansichten

**Ziel:** In dieser Übung erstellen Sie eine neue Ansicht, die später in modellgesteuerten Apps verwendet werden kann.

### Aufgabe Nr. 1: Bearbeiten der verschiedenen Ansichten für Spesenzeilen

1. Falls noch nicht geschehen, melden Sie sich bei  `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie nicht bereits ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen und öffnen Sie die Tabelle „Spesenzeile“.
6. Wählen Sie unter Datenerfahrungen **Ansichten** aus.
7. Öffnen Sie die Ansicht **Aktive Spesenzeilen**.
8. Klicken Sie auf **Spalte anzeigen.** Wählen Sie **Spesendatum, Artikelbeschreibung, Spesentyp** und **Spesenbetrag** aus.
9. Suchen Sie die Spalte **Erstellt am** und markieren Sie sie. Wählen Sie im angezeigten Menü **Entfernen.**
10. Ihre Ansicht sollte die Spalten „Spesentitel“, „Spesendatum“, „Artikelbeschreibung“, „Spesentyp“ und „Spesenbetrag“ enthalten.
11. Wählen Sie die Schaltfläche **Speichern und veröffentlichen**.
12. Wählen Sie die Schaltfläche „Zurück“, um zur Liste der Ansichten zurückzukehren.

Als Nächstes wiederholen wir diesen Vorgang, um die dazugehörige Spesenzeilenansicht zu aktualisieren. Dies ist die Ansicht, die angezeigt wird, wenn Sie Spesenzeilen aus einer übergeordneten Tabelle wie „Spesenabrechnung“ betrachten.

### Aufgabe Nr. 2: Aktualisieren der dazugehörigen Spesenzeilenansicht 

1. Suchen und öffnen Sie die dazugehörige Spesenzeilenansicht.
2. Klicken Sie auf **Spalte anzeigen.** Wählen Sie **Spesendatum, Artikelbeschreibung, Spesentyp** und **Spesenbetrag** aus.
3. Suchen Sie die Spalte **Erstellt am** und markieren Sie sie. Wählen Sie im angezeigten Menü **Entfernen.**
4. Ihre Ansicht sollte die Spalten „Spesentitel“, „Spesendatum“, „Artikelbeschreibung“, „Spesentyp“ und „Spesenbetrag“ enthalten.
5. Wählen Sie die Schaltfläche **Speichern und veröffentlichen**.
6. Wählen Sie die Schaltfläche „Zurück“, um zur Liste der Ansichten zurückzukehren.

Schließlich wiederholen wir diesen Vorgang noch einmal, um die Ansicht „Aktive Spesenzeilen schnell finden“ zu aktualisieren. Dies ist die Ansicht, die verwendet wird, wenn ein Benutzer bzw. eine Benutzerin das Suchfeld verwendet, um nach einer bestimmten Spesenzeile zu suchen.

### Aufgabe Nr. 3: Aktualisieren der Ansicht für die Schnellsuche

1. Suchen Sie die Ansicht „Aktive Spesenzeilen schnell finden“ und öffnen Sie sie.
2. Klicken Sie auf **Spalte anzeigen.** Wählen Sie **Spesendatum, Artikelbeschreibung, Spesentyp** und **Spesenbetrag** aus.
3. Suchen Sie die Spalte **Erstellt am** und markieren Sie sie. Wählen Sie im angezeigten Menü **Entfernen.**
4. Ihre Ansicht sollte die Spalten „Spesentitel“, „Spesendatum“, „Artikelbeschreibung“, „Spesentyp“ und „Spesenbetrag“ enthalten.
5. Wählen Sie auf der rechten Seite des Bildschirms im Abschnitt „Suchen nach“ die Option **Spalten der Suchtabelle bearbeiten** aus.
6. Fügen Sie die folgenden Spalten hinzu:
    - Spesendatum
    - Spesentyp
7. Wählen Sie die Schaltfläche **Anwenden** aus.
8. Wählen Sie die Schaltfläche **Speichern und veröffentlichen**.
9. Wählen Sie die Schaltfläche „Zurück“, um zur Liste der Ansichten zurückzukehren.

### Aufgabe Nr. 4: Bearbeiten der verschiedenen Spesenabrechnungsansichten

1. Falls noch nicht geschehen, melden Sie sich bei  `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie nicht bereits ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen und öffnen Sie die Tabelle „Spesenabrechnung“ aus.
6. Wählen Sie unter Datenerfahrungen **Ansichten** aus.
7. Öffnen Sie die Ansicht **Aktive Spesenabrechnungen**.
8. Klicken Sie auf **Spalte anzeigen.** Wählen Sie **Berichtszweck, Berichtsfälligkeitsdatum, Berichtssumme** und **Letztes Datum für die Genehmigung** aus.
9. Suchen Sie die Spalte **Erstellt am** und markieren Sie sie. Wählen Sie im angezeigten Menü **Entfernen.**
10. In Ihrer Ansicht sollten die Spalten „Berichtszweck“, „Berichtsfälligkeitsdatum“, „Berichtssumme“ und „Letztes Datum für die Genehmigung“ angezeigt werden.
11. Wählen Sie die Schaltfläche **Speichern und veröffentlichen**.
12. Wählen Sie die Schaltfläche „Zurück“, um zur Liste der Ansichten zurückzukehren.

Als Nächstes wiederholen wir diesen Vorgang, um die Ansicht „Inaktive Spesenabrechnungen“ zu aktualisieren.

### Aufgabe Nr. 5: Aktualisieren der Ansicht „Inaktive Spesenabrechnungen“

1. Suchen und öffnen Sie die Ansicht „Inaktive Spesenabrechnungen“.
2. Klicken Sie auf **Spalte anzeigen.** Wählen Sie **Berichtszweck, Berichtsfälligkeitsdatum, Berichtssumme** und **Letztes Datum für die Genehmigung** aus.
3. Suchen Sie die Spalte **Erstellt am** und markieren Sie sie. Wählen Sie im angezeigten Menü **Entfernen.**
4. In Ihrer Ansicht sollten die Spalten „Berichtszweck“, „Berichtsfälligkeitsdatum“, „Berichtssumme“ und „Letztes Datum für die Genehmigung“ angezeigt werden.
5. Wählen Sie die Schaltfläche **Speichern und veröffentlichen**.
6. Wählen Sie die Schaltfläche „Zurück“, um zur Liste der Ansichten zurückzukehren.

### Aufgabe Nr. 6: Aktualisieren der Ansicht „Schnellsuche der aktiven Spesenabrechnungen“ 

Schließlich wiederholen wir diesen Vorgang noch einmal, um die Ansicht „Schnellsuche der aktiven Spesenabrechnungen“ zu aktualisieren. Dies ist die Ansicht, die verwendet wird, wenn ein Benutzer bzw. eine Benutzerin das Suchfeld verwendet, um nach einer bestimmten Spesenabrechnung zu suchen.

1. Suchen und öffnen Sie die Ansicht „Schnellsuche der aktiven Spesenabrechnungen“.
2. Klicken Sie auf **Spalte anzeigen.** Wählen Sie **Berichtszweck, Berichtsfälligkeitsdatum, Berichtssumme** und **Letztes Datum für die Genehmigung** aus.
3. Suchen Sie die Spalte **Erstellt am** und markieren Sie sie. Wählen Sie im angezeigten Menü **Entfernen.**
4. In Ihrer Ansicht sollten die Spalten „Berichtszweck“, „Berichtsfälligkeitsdatum“, „Berichtssumme“ und „Letztes Datum für die Genehmigung“ angezeigt werden.
5. Wählen Sie auf der rechten Seite des Bildschirms im Abschnitt „Suchen nach“ die Option **Spalten der Suchtabelle bearbeiten** aus.
6. Fügen Sie die Spalte „Berichtszweck“ hinzu.
7. Wählen Sie die Schaltfläche **Anwenden** aus.
8. Wählen Sie die Schaltfläche **Speichern und veröffentlichen**.
9. Wählen Sie die Schaltfläche „Zurück“, um zur Liste der Ansichten zurückzukehren.

### Aufgabe Nr. 7: Erstellen einer neuen Ansicht namens „Heute fällige Spesenabrechnungen“

1. Falls noch nicht geschehen, melden Sie sich bei  `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie nicht bereits ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen und öffnen Sie die Tabelle „Spesenabrechnung“ aus.
6. Wählen Sie unter Datenerfahrungen **Ansichten** aus.
7. Öffnen Sie die Ansicht „Aktive Spesenabrechnungen“.
8. Wählen Sie die Schaltfläche **Speichern unter** aus.
9. Ändern Sie den Namen in *`Expense Reports Due Today`*.
10. Wählen Sie die Schaltfläche **Speichern** aus.
11. Wählen Sie im Abschnitt „Filtern nach“ die Option **Filter bearbeiten** aus.
12. Wählen Sie die Schaltfläche **Hinzufügen** aus. Wählen Sie im angezeigten Menü **Zeile hinzufügen** aus.
13. Wählen Sie den Dropdownpfeil in der ersten leeren Zeile aus. Wählen Sie aus dem angezeigten Menü die Spalte **Berichtsfälligkeitsdatum**.
14. Ändern Sie das Feld „Entspricht“ in **Heute.**
15. Wählen Sie die Schaltfläche **OK** aus.
16. Wählen Sie die Schaltfläche **Speichern und veröffentlichen** aus.
