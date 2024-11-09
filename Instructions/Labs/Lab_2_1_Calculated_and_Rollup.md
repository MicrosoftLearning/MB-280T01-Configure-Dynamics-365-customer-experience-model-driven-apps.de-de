---
lab:
  title: 'Lab 2.1: Erstellen von berechneten Feldern und Rollupfeldern'
---

# Lab 2.1: Erstellen von berechneten Feldern und Rollupfeldern 

## Szenario
Das Bellows College ist eine Bildungsorganisation mit mehreren Campusgebäuden. Viele der Lehrer und Administratoren am Bellow College müssen an Veranstaltungen teilnehmen und Artikel kaufen. Historisch gesehen war die Nachverfolgung dieser Ausgaben eine Herausforderung.
Die Campusverwaltung möchte ihr Spesenabrechnungssystem modernisieren, indem den Mitarbeitern eine digitale Möglichkeit zum Melden von Ausgaben an die Hand gegeben wird.
Im Idealfall möchten sie, dass ihre Benutzenden nach jedem Ereignis oder Kauf eine Spesenabrechnung abschließen. Für jede Spesenabrechnung sollen sie einzelne Spesenpositionen hinzufügen können. Sie haben bereits damit begonnen, an dieser Lösung zu arbeiten. Die Tabelle „Expense Report“ wurde erstellt. Sie wurden aufgefordert, das Projekt zu übernehmen und abzuschließen.

## Weiterführende Schritte des Lab
Nach erfolgreichem Abschluss dieses Labs können Sie Folgendes:
- Einer vorhandenen Tabelle neue Felder hinzufügen
- Ein Rollupfeld erstellen
- Ein Berechnungsfeld erstellen

## Voraussetzungen
- Abschluss von Modul 1 Lab 0 – Überprüfen der Lab-Umgebung und Lab 1.1, in der Sie die Spesenabrechnungslösung importiert haben

## Vor dem Beginn zu beachtende Dinge
- Namenskonventionen: Geben Sie Namen sorgfältig ein.

## Übung 1: Erstellen von berechneten Feldern und Rollupfeldern
**Ziel:** In dieser Übung erstellen Sie ein Rollup und ein berechnetes Feld in der Tabelle der Spesenabrechnung.

### Aufgabe Nr. 1: Hinzufügen eines Rollupfelds zur Tabelle „Spesenabrechnung“
1. Navigieren Sie zum Power Apps Maker-Portal wenn nötig.
2. Stellen Sie sicher, dass Sie in der Umgebung arbeiten, in die Sie in der letzten Übung die Lösung „Expense Report“ importiert haben.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Suchen und wählen Sie die Lösung „Spesenabrechnung“ aus.
5. Suchen und öffnen Sie die Tabelle „Spesenabrechnung“ aus.
6. Wählen Sie in der Gruppe „Schema“ **Spalten** aus.
7. Wählen Sie **+Neue Spalte** aus.
8. Geben Sie für Anzeigename *`Report Total`* ein.
9. Wählen Sie **Währung** als Datentyp aus.
10. Wählen Sie in „Erforderlich“ die Option **Optional** aus.
11. Wählen Sie im Feld „Verhalten“ **Rollup** aus.
12. Wählen Sie die Schaltfläche **Speichern** aus. (Sie müssen die Spalte speichern, bevor Sie sie konfigurieren können.)
13. Nachdem die Spalte gespeichert wurde, sollte ein Popupfenster angezeigt werden. (Wenn Sie keine Popupnachricht erhalten, müssen Sie möglicherweise Popups zulassen.)
14. Wählen Sie unter „VERWANDTE ENTITÄT“ die Option **+ Verwandte Entität hinzufügen** aus.
15. Wählen Sie **(Spesenpositionen) Spesenabrechnung** aus.
16. Wählen Sie die Schaltfläche „Häkchen“, um die Änderung zu akzeptieren.
17. Wählen Sie unter „AGGREGATION“ die Option **+ Aggregation hinzufügen** aus.
18. Setzen Sie die Aggregatfunktion auf **Summe**.
19. Setzen Sie das Feld „aggregierte verwandte Entität“ auf **Spesenzeilen (Spesenabrechnung)**.
20. Markieren Sie das grüne Häkchen und wählen Sie dann die Schaltfläche **Speichern und Schließen**.

### Aufgabe Nr. 2: Hinzufügen eines berechneten Power Fx-Formel-Felds zur Tabelle „Spesenabrechnung“
1. Navigieren Sie zum Power Apps Maker-Portal wenn nötig.
2. Stellen Sie sicher, dass Sie in der Umgebung arbeiten, in die Sie in der letzten Übung die Lösung „Expense Report“ importiert haben.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Suchen und wählen Sie die Lösung „Spesenabrechnung“ aus.
5. Suchen und öffnen Sie die Tabelle „Spesenabrechnung“ aus.
6. Wählen Sie in der Gruppe „Schema“ **Spalten** aus.
7. Wählen Sie **+Neue Spalte** aus.
8. Geben Sie für Anzeigename *`Last Date for approval`* ein.
9. Wählen Sie für Datentyp **Formel** aus.
10. Geben Sie die folgende Formel ein:`DateAdd('Report Due Date',2)`
11. Legen Sie das Feld „Format“ auf **Nur Datum** fest.
12. Wählen Sie die Schaltfläche **Speichern** aus. (Sie müssen die Spalte speichern, bevor Sie sie konfigurieren können.)
