---
lab:
  title: "Lab\_4.4: Erstellen einer modellgesteuerten App"
---

# Lab 4.4: Erstellen einer modellgesteuerten App

## Szenario
Das Bellows College ist eine Bildungsorganisation mit mehreren Campusgebäuden.

Viele der Lehrer und Administratoren am Bellow College müssen an Veranstaltungen teilnehmen und Artikel kaufen. Historisch gesehen war die Nachverfolgung dieser Ausgaben eine Herausforderung.
Die Campusverwaltung möchte ihr Spesenabrechnungssystem modernisieren, indem den Mitarbeitern eine digitale Möglichkeit zum Melden von Ausgaben an die Hand gegeben wird.

Während dieses Kurses erstellen Sie Anwendungen und führen Automatisierung durch, damit die Mitarbeitenden des Bellows College Ausgaben verwalten können.

## Weiterführende Schritte des Lab
Im Rahmen der Konfiguration der modellgesteuerten App führen Sie Folgendes aus:
- Konfigurieren Ihrer neuen modellgesteuerten App mit dem Namen „Mitarbeiterspesenverwaltung“

Wir werden mit folgenden Komponenten arbeiten:
- Ansichten: Mithilfe von Ansichten kann der Benutzer die vorhandenen Daten in Form einer Tabelle anzeigen.
- Formulare: Hier erstellt bzw. aktualisiert der Benutzer neue Zeilen in den Tabellen.
Beide werden für eine bessere Benutzererfahrung in die modellgesteuerte App integriert.

## Voraussetzungen
- Beendigung von Modul 1 Lab 0 – Lab-Umgebung überprüfen

## Übung 1: Erstellen einer modellgesteuerten App
**Ziel:** In dieser Übung verwenden Sie die modellgesteuerte App, die Sie in Lab 4.3 konfiguriert haben. Anschließend passen Sie die Sitemap an und testen die App.
Der Einfachheit halber und aus Zeitgründen gehen wir in diesem Lab nicht auf alle Spalten der Spesenabrechnung ein.

## Aufgabe 1: Konfigurieren der Sitemap
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen Sie die *`Employee Expense Management`*-Anwendung, die Sie in der letzten Übung erstellt haben.
6. Wählen Sie **Bearbeiten** aus, um den modernen App-Designer zu öffnen.
7. Wählen Sie in der Befehlsleiste **+Seite hinzufügen** aus.
8. Der Bildschirm **Neue Seite hinzufügen** wird geöffnet.
9. Wählen Sie **Dataverse-Tabelle** aus.
10. Wählen Sie die folgenden Tabellen aus:
    - Spesenabrechnung
    - Spesenposition
11. Stellen Sie sicher, dass im Navigationsbereich „Anzeigen“ ausgewählt ist.
12. Nachdem Sie die beiden Tabellen ausgewählt haben, wählen Sie **Hinzufügen** aus.
13. Wählen Sie unter „Navigation“ das Formular **Spesenabrechnungen** aus.
14. Wechseln Sie auf der rechten Seite des Bildschirms zum Abschnitt „In dieser App“.
15. Wählen Sie **Mehr anzeigen** aus.
16. Wählen Sie die **Auslassungspunkte** neben dem Schnellansichtsformular für Informationen aus.
17. Wählen Sie im eingeblendeten Menü **Entfernen** aus.
18. Wählen Sie die **Auslassungspunkte** neben dem Informationskartenformular aus.
19. Wählen Sie im eingeblendeten Menü **Entfernen** aus.
20. Wählen Sie unter „Navigation“ das Formular **Spesenpositionen** aus.
21. Wechseln Sie auf der rechten Seite des Bildschirms zum Abschnitt „In dieser App“.
22. Wählen Sie **Mehr anzeigen** aus.
23. Wählen Sie die **Auslassungspunkte** neben dem Schnellansichtsformular für Informationen aus.
24. Wählen Sie im eingeblendeten Menü **Entfernen** aus.
25. Wählen Sie die **Auslassungspunkte** neben dem Informationskartenformular aus.
26. Wählen Sie im eingeblendeten Menü **Entfernen** aus.
27. Klicken Sie auf **Speichern**, und warten Sie, bis die Änderungen gespeichert sind.
28. Nachdem der Speichervorgang abgeschlossen wurde, wählen Sie die Schaltfläche **Veröffentlichen** aus, um Ihre Änderungen zu veröffentlichen. Warten Sie darauf, bis die Veröffentlichung abgeschlossen ist.

### Aufgabe 2: Testen der App
**Starten der Anwendung**
1. Wählen Sie die Schaltfläche Wiedergeben aus. Die modellgesteuerte App wird auf einer neuen Registerkarte geladen.

**Erstellen einer neuen Spesenabrechnung**
1. Wählen Sie in der linken Navigationsleiste (auch „Siteübersicht“ genannt) **Spesenabrechnungen** aus.
2. Wählen Sie **+ Neu** aus.
3. Füllen Sie die Felder wie folgt aus:
    - Berichtsname: **`New Test Report`**
    - Berichtszweck: Wählen Sie **`Conference`** aus
    - Fälligkeitsdatum melden: Wählen Sie **`Today's date`** aus
4. Wählen Sie **Speichern und schließen** aus. Dadurch wird der neue Testbericht erstellt, und Sie sollten ihn in der Ansicht Aktive Spesenabrechnungen anzeigen können.
5. Ändern Sie die Ansicht in **Heute fällige Spesenabrechnungen** über die Dropdownliste neben Aktive Spesenabrechnungen.
6. Sie können weitere Testdatensätze hinzufügen.

Ihre modellgesteuerte App sollte ungefähr folgendermaßen aussehen:

![Ein Screenshot des Bildschirms der modellgesteuerten App.](./Media/Model_driven_apps.png)

Herzlichen Glückwunsch! Sie haben Ihre erste modellgesteuerte App erstellt und konfiguriert.
