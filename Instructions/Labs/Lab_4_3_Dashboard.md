---
lab:
  title: "Lab\_4.3: Erstellen eines Dashboards"
---

# Lab 4.3: Erstellen eines Dashboards 

## Szenario
Das Bellows College ist eine Bildungsorganisation mit mehreren Campusgebäuden. Viele der Lehrer und Administratoren am Bellow College müssen an Veranstaltungen teilnehmen und Artikel kaufen. Historisch gesehen war die Nachverfolgung dieser Ausgaben eine Herausforderung.
Die Campusverwaltung möchte ihr Spesenabrechnungssystem modernisieren, indem den Mitarbeitern eine digitale Möglichkeit zum Melden von Ausgaben an die Hand gegeben wird.
Während dieses Kurses erstellen Sie Anwendungen und führen Automatisierung durch, damit die Mitarbeitenden des Bellows College Ausgaben verwalten können.

## Weiterführende Schritte des Lab
Nach erfolgreichem Abschluss dieses Labs können Sie Folgendes:
- Eine neue modellgesteuerte App erstellen
- Erstellen eines persönlichen Dashboards, in dem Spesenabrechnungsinformationen angezeigt werden
- Hinzufügen von Ansichten und Dashboards zu Ihrer modellgesteuerten App

## Voraussetzungen
- Beendigung von Modul 1 Lab 0 – Lab-Umgebung überprüfen

## Übung 1: Erstellen eines persönlichen Dashboards

### Aufgabe 1: Erstellen Sie Ihre neue modellgesteuerte App
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Wählen Sie auf der Befehlsleiste die Schaltfläche **+ Neu** aus.
6. Wechseln Sie im daraufhin angezeigten Menü zu **App > modellgesteuerte App.**
7. Geben Sie *`Employee Expense Management`* als Name ein, und wählen Sie **Erstellen** aus.

### Aufgabe 2: Erstellen einer neuen Ansicht namens „Meine aktiven Spesenabrechnungen“
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Suchen und öffnen Sie die Tabelle „Spesenabrechnung“ aus.
6. Wählen Sie unter Datenerfahrungen **Ansichten** aus.
7. Öffnen Sie die Ansicht **Aktive Spesenabrechnungen**.
8. Wählen Sie die Schaltfläche **Speichern unter** aus.
9. Ändern Sie den Namen in *`My Active Expense Reports`*.
10. Wählen Sie die Schaltfläche **Speichern** aus.
11. Wählen Sie im Abschnitt „Filtern nach“ die Option **Filter bearbeiten** aus.
12. Wählen Sie die Schaltfläche **Hinzufügen** aus. Wählen Sie im angezeigten Menü **Zeile hinzufügen** aus.
13. Wählen Sie den Dropdownpfeil in der ersten leeren Zeile aus. Wählen Sie im daraufhin angezeigten Menü die Spalte **Besitzende Person** aus.
14. Ändern Sie das Feld **Gleich** in „Gleich der aktuellen besitzenden Person“.
15. Wählen Sie die Schaltfläche **OK** aus.
16. Wählen Sie die Schaltfläche **Speichern und veröffentlichen** aus.

### Aufgabe 3: Hinzufügen eines Dashboards-Abschnitts zur Mitarbeiterspesenverwaltungs-App
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei https://make.powerapps.com an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Wählen Sie **Apps** aus.
6. Suchen Sie die Mitarbeiterspesenverwaltungs-App.
7. Wählen Sie die **Vertikalen Auslassungspunkte** und im erscheinenden Menü **Bearbeiten** aus.
8. Wählen Sie die Schaltfläche **Seite hinzufügen** aus.
9. Wählen Sie **Dashboard** aus.
10. Erkunden Sie die standardmäßig verfügbaren Systemdashboards. Wenn Sie fertig sind, wählen Sie eines der Dashboards aus, das Sie zu Ihrer App hinzufügen möchten.
11. Wählen Sie **Hinzufügen**.
12. Wenn „Neue Gruppe“ ausgewählt ist, ändern Sie den Titel in **Dashboards.**
13. Wählen Sie die Schaltfläche **Speichern** aus.
14. Nachdem der Speichervorgang abgeschlossen wurde, klicken Sie auf die Schaltfläche **Speichern und veröffentlichen**.

### Aufgabe 4: Hinzufügen eines persönlichen Dashboards zur Mitarbeiterspesenverwaltungs-App
1. Wenn Sie noch nicht angemeldet sind, melden Sie sich bei `https://make.powerapps.com` an.
2. Wählen Sie oben rechts die Umgebung aus, in die Sie die Spesenabrechnungslösung importiert haben, falls sie noch nicht ausgewählt ist.
3. Wählen Sie links im Navigationsbereich die Option **Lösungen** aus.
4. Öffnen Sie die Spesenabrechnungslösung.
5. Wählen Sie **Apps** aus.
6. Suchen Sie die modellgesteuerte Mitarbeiterspesenverwaltungs-App.
7. Wählen Sie die **vertikalen Auslassungspunkte** aus. Wählen Sie im angezeigten Menü die Option **Wiedergeben** aus.
8. Wählen Sie in der Gruppe „Dashboards“ das Systemdashboard aus, das Sie in Aufgabe 3 hinzugefügt haben.
9. Wählen Sie die Schaltfläche **Neu** aus.
10. Wählen Sie im angezeigten Menü **Dynamics 365 Dashboard** aus.
11. Wählen Sie die Option **Zweispaltiges reguläre Dashboard** aus.
12. Wählen Sie die Schaltfläche **Erstellen**.
13. Ändern Sie den Dashboardnamen in *`Expense Report Dashboard`*.
14. Wählen Sie im Abschnitt oben links das **Listensymbol** aus.
15. Konfigurieren Sie die Liste wie folgt:
    - Datensatztyp: Spesenabrechnungen
    - Ansicht: Heute fällige Spesenabrechnungen.
16. Wählen Sie die Schaltfläche **Hinzufügen** aus.
17. Wählen Sie im Abschnitt oben rechts das **Suchsymbol** aus.
18. Konfigurieren Sie die Liste wie folgt:
    - Datensatztyp: Spesenabrechnungen
    - Ansicht: Meine aktiven Spesenabrechnungen.
19. Wählen Sie die Schaltfläche **Hinzufügen** aus.
20. Wählen Sie im Abschnitt unten links das **Listensymbol** aus.
21. Konfigurieren Sie die Liste wie folgt:
    - Datensatztyp: Spesenpositionen
    - Ansicht: Meine aktiven Spesenpositionen.
22. Wählen Sie die Schaltfläche **Hinzufügen** aus.
23. Wählen Sie im Abschnitt unten rechts das **Listensymbol** aus.
24. Konfigurieren Sie die Liste wie folgt:
    - Datensatztyp: Kontakte
    - Ansicht: Meine aktiven Kontakte.
25. Wählen Sie die Schaltfläche **Hinzufügen** aus.
26. Wählen Sie die Schaltfläche **Speichern** in der oberen linken Ecke.
27. Sobald das Dashboard gespeichert ist, wählen Sie die Schaltfläche **Schließen** aus.
28. Sie sollten zum Dashboard zur Spesenabrechnung weitergeleitet werden.
29. Wählen Sie in der Befehlsleiste oben **Als Standard festlegen.**
