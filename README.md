[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=4100856&assignment_repo_type=AssignmentRepo)
# Übungsblatt 4

## WebGIS Anwendung zur Bürgerbeteiligung

In diesem Übungsblatt erstellen wir eine WebGIS-Anwendung, die es Benutzern ermöglicht, Gebäude auf einer vorgegebenen Bebauungsfläche zu positionieren. Dabei stehen dem Benutzer 10 vorgefertigte Grundrisse zur Verfügung.

## 1) Basiskarte (10 Punkte)

### a) Erstellen einer OpenLayers Karte mit OSM Hintergrundlayer (1 P)

### b) Einbinden des WMS Tilelayers (1 P)
- **URL:** [http://osmatrix.geog.uni-heidelberg.de:8080/geoserver-2.18/mauer/wms](http://osmatrix.geog.uni-heidelberg.de:8080/geoserver-2.18/mauer/wms)
- **Layername:** mauer:ub4_baugebiet

### c) Die Bürgerkarte soll in der Projektion WGS84/UTM 32N dargestellt werden. Dazu benötigen Sie:
- den richtigen EPSG Code (1 P)
- den proj4js Definitionsstring z.B. von https://epsg.io (1 P)
- binden Sie die Zusatzbibliothek proj4js in ihre Webseite ein und registrieren Sie die oben genannte Projektion (3 P)
- Konfigurieren Sie ihren Map-View so, dass zoom und center entsprechend auf das Baugebiet zeigen (3 P)

## 2) Interaktionslayer (10 Punkte)

Um den Bürgern eine Interaktion mit der Karte zu ermöglichen, benötigen wir einen Vektorlayer, der über eine WFS URL eingebunden wird.

### a) Binden Sie folgenden Layer vom Geoserver als VectorLayer (WFS mit GeoJSON Format) ein: (5 P)
- mauer:ub4_bebauung

### b) Fügen Sie Ihrer Karte zwei OpenLayers Interaction hinzu, so dass Sie einzelne Feature des Layers
mauer:ub4_bebauung „selektieren“ (select) und „verschieben“ (translate) können. (5 P)

