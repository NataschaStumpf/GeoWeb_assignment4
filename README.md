[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=4100856&assignment_repo_type=AssignmentRepo)
# Übungsblatt 4

## WebGIS Anwendung zur Bürgerbeteiligung

In diesem Übungsblatt erstellen wir eine WebGIS-Anwendung, die es Benutzern ermöglicht, Gebäude auf einer vorgegebenen Bebauungsfläche zu positionieren. Dabei stehen dem Benutzer 10 vorgefertigte Grundrisse zur Verfügung.

## 1) Basiskarte (10 Punkte)

### a) Erstellen einer OpenLayers Karte mit OSM Hintergrundlayer (1 P)

### b) Einbinden des WMS Tilelayers (1 P)
- **URL:** [http://osmatrix.geog.uni-heidelberg.de:8080/geoserver-2.18/mauer/wms](http://osmatrix.geog.uni-heidelberg.de:8080/geoserver-2.18/mauer/wms)
- **Layername:** mauer:ub4_baugebiet

### c) Projektion WGS84/UTM 32N (6 P)
- **EPSG Code:** [Fügen Sie den EPSG-Code ein]
- **proj4js Definitionsstring:** [Fügen Sie den proj4js Definitionsstring ein]
- **Zusatzbibliothek proj4js:** Geben Sie an, wie Sie die proj4js-Bibliothek in Ihre Webseite eingebunden und die Projektion registriert haben.
- **Konfiguration des Map-View:** Stellen Sie sicher, dass Zoom und Zentrum auf das Baugebiet ausgerichtet sind.

## 2) Interaktionslayer (10 Punkte)

Um den Bürgern eine Interaktion mit der Karte zu ermöglichen, benötigen wir einen Vektorlayer, der über eine WFS URL eingebunden wird.

### a) Einbinden des VectorLayers (WFS mit GeoJSON Format) (5 P)
- **Layername:** mauer:ub4_bebauung

### b) Hinzufügen von OpenLayers Interaktionen (5 P)
- Fügen Sie Ihrer Karte zwei OpenLayers Interaction hinzu, um einzelne Feature des Layers "mauer:ub4_bebauung" auszuwählen (select) und zu verschieben (translate).

Bitte beachten Sie, dass die Punktevergabe den jeweiligen Aufgaben entspricht.
