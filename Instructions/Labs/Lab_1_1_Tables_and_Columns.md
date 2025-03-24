---
lab:
  title: 'Lab 1.1: Erstellen und Verwalten von Tabellen und Spalten'
---

# Lab 1.1: Erstellen und Verwalten von Tabellen und Spalten

## Szenario
Das Bellows College ist eine Bildungsorganisation mit mehreren Campusgebäuden. Viele der Lehrer und Administratoren am Bellow College müssen an Veranstaltungen teilnehmen und Artikel kaufen. Historisch gesehen war die Nachverfolgung dieser Ausgaben eine Herausforderung.
Die Campusverwaltung möchte ihr Spesenabrechnungssystem modernisieren, indem den Mitarbeitern eine digitale Möglichkeit zum Melden von Ausgaben an die Hand gegeben wird.
Im Idealfall möchten sie, dass ihre Benutzenden nach jedem Ereignis oder Kauf eine Spesenabrechnung abschließen. Für jede Spesenabrechnung sollen sie einzelne Spesenpositionen hinzufügen können. Sie haben bereits damit begonnen, an dieser Lösung zu arbeiten. Die Tabelle „Expense Report“ wurde erstellt. Sie wurden aufgefordert, das Projekt zu übernehmen und abzuschließen.

## Weiterführende Schritte des Lab
Nach erfolgreichem Abschluss dieses Labs können Sie Folgendes:
- Importieren einer Lösung in Ihre Umgebung, die die Spesenberichtstabelle enthält.
- Erstellen einer Spesenzeilentabelle
- Fügen Sie der Tabelle „Spesenzeile“ die erforderlichen Spalten hinzu.
- Fügen Sie einige Beispieldaten hinzu.

## Voraussetzungen
- Beendigung von Modul 1 Lab 0 – Lab-Umgebung überprüfen

## Vor dem Beginn zu beachtende Dinge
- Namenskonventionen: Geben Sie Namen sorgfältig ein.

## Übung 1: Importieren der Spesenabrechnungslösung in Ihre Umgebung
**Ziel:** In dieser Übung importieren Sie die Spesenabrechnungslösung, die die Tabelle „Spesenabrechnung“ enthält.

### Aufgabe Nr. 1: Importieren der Lösung
Die Tabelle „Spesenabrechnung“ enthält Informationen über die Spesenabrechnung, die die Person übermittelt.
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich mit den Anmeldeinformationen Ihrer Umgebung an `make.powerapps.com`.
2. Stellen Sie sicher, dass Sie sich im Menü „Umgebung“ oben rechts in der Umgebung befinden, in die Sie die Lösung importieren möchten.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Wählen Sie in der Befehlsleiste oben **Lösung importieren** aus.
5. Wählen Sie die Schaltfläche **Durchsuchen** aus.
6. Suchen Sie die Datei der `ExpenseReport_1_0_0_1`-Lösung, die sich in Ihren Kursmaterialien befindet, und wählen Sie sie aus.
7. Wählen Sie die Schaltfläche **Importieren** aus.

*Hinweis: Es kann mehrere Minuten dauern, bis die Lösung in Ihre Umgebung importiert wird.*

## Übung 2: Erstellen benutzerdefinierter Tabellen und Spalten
**Ziel:** In dieser Übung importieren Sie die Spesenabrechnungslösung, die die Tabelle „Spesenabrechnung“ enthält.

### Aufgabe Nr. 1: Erstellen einer Spesenzeilentabelle
1. Navigieren Sie zum Power Apps Maker-Portal wenn nötig.
2. Stellen Sie sicher, dass Sie in der Umgebung arbeiten, in die Sie die `ExpenseReport_1_0_0_1`-Lösung während der letzten Übung importiert haben.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Suchen und wählen Sie die Lösung „Spesenabrechnung“ aus.
5. Wählen Sie die Schaltfläche **Neu** aus.
6. Gehen Sie im angezeigten Menü zu **Tabelle.** Wählen Sie als Nächstes **Tabelle (erweiterte Eigenschaften)** aus.
7. Konfigurieren Sie Ihre neue Tabelle wie folgt:
   - Anzeigename: `Expense Line`
   - Pluralname: `Expense Lines`
   - Anlagen aktivieren (einschließlich Notizen und Dateien): Ausgewählt
8. Wählen Sie die Registerkarte „Primäre Spalte“ aus und ändern Sie den Anzeigenamen in „Spesentitel“.
9. Wählen Sie die Schaltfläche Speichern aus.

*Hinweis: Die Erstellung der Tabelle kann ein bis zwei Minuten dauern.*

### Aufgabe 2: Hinzufügen der erforderlichen Spalten zur Tabelle „Spesenposition“
1. Wählen Sie bei geöffneter Tabelle „Spesenposition“ in der Gruppe „Schema“ die Option „Spalten“ aus.
2. Wählen Sie **+ Neue Spalte** aus.
3. Geben Sie für Anzeigename **`Expense Type`** ein.
4. Wählen Sie **Auswahl > Auswahl** für „Datentyp“ aus.
5. Wählen Sie in „Erforderlich“ die Option **Optional** aus.
6. Legen Sie „Synchronisierung mit globaler Auswahl“ auf **Ja (empfohlen)** fest.
7. Wählen Sie unter „Synchronisieren dieser Auswahl mit Feld“ die Option **+ Neue Auswahlmöglichkeit** aus.
8. Geben Sie im Feld „Anzeigename“ *`Expense Type`* ein.
9. Geben Sie im Feld „Beschriftung“ für die erste Auswahl *`Meals`* ein.
10. Wählen Sie **+ Neue Auswahl** aus.
11. Geben Sie im Feld „Beschriftung“ *`Lodging`* ein.
12. Wiederholen Sie die Schritte 10 und 11, um die folgenden Optionen hinzuzufügen:
    - `Travel`
    - `Entertainment`
    - `Supplies / Equipment`
    - `Other`
13. Wählen Sie die Schaltfläche **Speichern** aus.
14. Wählen Sie unter „Diese Auswahl mit Feld synchronisieren“ die Auswahl **Spesentyp** aus, die Sie gerade erstellt haben.
15. Stellen Sie das Feld „Standardauswahl“ auf **Keine**ein.
16. Wählen Sie **Speichern**.

### Aufgabe 3: Erstellen der Spalte „Spesenbetrag“
1. Wählen Sie + Neue Spalte aus.
2. Geben Sie für Anzeigename `Expense Amount` ein.
3. Wählen Sie Währung als Datentyp aus.
4. Wählen Sie Speichern.

### Aufgabe 4: Erstellen der Spalte „Elementbeschreibung“
1. Wählen Sie **+ Neue Spalte** aus.
2. Geben Sie für Anzeigename *`Item Description`* ein.
3. Wählen Sie für den Datentyp **Mehrere Textzeilen > Nur-Text** aus.
4. Wählen Sie **Speichern**.

### Aufgabe 5: Erstellen der Spalte „Spesendatum“
1. Wählen Sie **+ Neue Spalte** aus.
2. Geben Sie *`Expense Date`* für den Anzeigenamen ein.
3. Wählen Sie **Nur Datum** aus der Gruppe „Datum und Uhrzeit“ im Feld „Datentyp“ aus.
4. Erweitern Sie **Erweiterte Optionen**.
5. Setzen Sie das Feld „Zeitzonenanpassung“ auf **Ortszeit Benutzender** fest.
6. Wählen Sie **Speichern**.

### Aufgabe 6: Erstellen einer Kostenabrechnungsspalte
1. Wählen Sie **+ Neue Spalte** aus.
2. Geben Sie *`Expense Report`* für den Anzeigenamen ein.
3. Wählen Sie **Lookup** aus der Lookup-Gruppe im Feld „Datentyp“ aus.
4. Wählen Sie im Feld „Verwandte Tabelle“ die Option **Spesenabrechnung** aus.
5. Wählen Sie **Speichern**.

## Übung 3: Tabelle bearbeiten
**Ziel:** In dieser Übung ändern Sie manuell eine Tabelle.

### Aufgabe Nr. 1: Ändern Sie die angezeigten Spalten
1. Navigieren Sie zum Power Apps Maker-Portal wenn nötig.
2. Stellen Sie sicher, dass Sie in der Umgebung arbeiten, in der Sie die Lösung **ExpenseReport_1_0_0_1** während der letzten Übung importiert haben.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Suchen und wählen Sie die Lösung **Spesenabrechnungen** aus.
5. Wählen Sie links im Navigationsbereich die Option **Tabellen** aus.
6. Öffnen Sie die Tabelle „Spesenposition“, die Sie in der vorherigen Übung erstellt haben.
7. Wählen Sie neben der Spalte „Sequenz importieren“ **+[X] mehr** aus. (Die hier gezeigte Zahl hängt von Ihrer Browsergröße ab.)
8. Wählen Sie im daraufhin angezeigten Menü die folgenden Spalten aus.
   - Spesenbetrag (Basis)
   - Spesendatum (Wenn nicht bereits ausgewählt)
   - Spesenabrechnung
   - Spesentyp
   - Ausgabenbetrag
   - Item Description
9. Wählen Sie die Schaltfläche **Speichern** aus.
10. Suchen Sie die Spalte **Erstellt von**, und wählen Sie sie aus.
11. Wählen Sie im angezeigten Menü **Ausblenden** aus.
12. Wiederholen Sie die Schritte 10 und 11, um die folgenden Spalten zu entfernen:
    - Erstellt von
    - Spesenposition
    - Importsequenz
