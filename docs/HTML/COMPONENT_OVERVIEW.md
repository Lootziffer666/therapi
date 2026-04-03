# THERAPI Prototype — Komponentenübersicht

Diese Übersicht ist aus dem aktuellen Prototyp abgeleitet und dient als verbindlicher Baukasten.

## 1. App Shell

### 1.1 Sidebar
Zweck:
- globale Primärnavigation

Bestandteile:
- Logo
- primäre Navigationspunkte
- klar abgesetzter unterer Abschluss / Settings-Bereich
- Footer-Status bzw. Systemkontext, sofern im jeweiligen Screen vorhanden

Verwendung:
- auf jeder produktiven Seite verpflichtend

Regeln:
- Breite `240px`
- links fixiert oder visuell als feste linke Spalte geführt
- aktive Seite farblich markiert
- kein alternatives Sidebar-Muster zulässig

### 1.2 Topbar
Zweck:
- systemische Zustände und Kontextindikatoren

Bestandteile:
- Status-Chips / Badges
- technische Kontextangaben
- ggf. Suche oder Utility-Aktionen
- visuell kompakte obere Leiste

Verwendung:
- auf jeder produktiven Seite verpflichtend

Regeln:
- Höhe `56px`
- keine Hero-Substitution
- kein zweites Topbar-Muster zulässig

### 1.3 Page Header
Zweck:
- Seitenkontext

Bestandteile:
- H1
- kurze Subline oder Kontexttext
- optional kleinere technische Meta-Angabe

Regeln:
- direkt unter der Topbar
- keine große Leerfläche davor
- H1-Stil ist systemisch festgelegt

---

## 2. Navigation

### 2.1 Standard Nav Item
Bestandteile:
- Material Symbol
- Textlabel

Zustände:
- default
- hover
- active

Regeln:
- Icon links, Text rechts
- aktiver Zustand petrolfarben
- aktive Fläche leicht getönt

### 2.2 Lower Navigation / Settings Zone
Zweck:
- Separation des unteren Bereichs

Regeln:
- feine Border oder klare Distanz
- kein alternatives Containerpattern nötig

---

## 3. Status-Komponenten

### 3.1 Status Chip
Beispiele:
- Proxy Status
- Base URL
- Modus-/Kontextindikatoren
- Monitoring-/Live-Hinweise

Regeln:
- kleine Kapsel
- niedrige Höhe
- semantischer, technischer Text
- ruhige Farben

### 3.2 Footer Status Tile
Zweck:
- Version / Systemstatus in Sidebar

Bestandteile:
- Kürzel-Kachel oder kompaktes Icon
- Versionsnummer
- kurzer Systemtext

---

## 4. Content-Container

### 4.1 Standard Card
Zweck:
- universelle Inhaltsfläche

Regeln:
- helle Fläche
- dezente Trennung
- mittlerer Radius
- funktionaler statt dekorativer Einsatz

### 4.2 Dense Info Panel
Zweck:
- Kennzahlen, kurze Beschreibungen, technische Details

Regeln:
- kompakte Innenabstände
- keine unnötige Höhe
- bevorzugt in Gruppen statt isoliert mit viel Leerraum

### 4.3 Split Layout
Zweck:
- Master/Detail oder Liste/Inspektor

Verwendung:
- Collections Export
- Capture Inspector
- Endpoint Explorer
- Schema Drift in seiner Hauptgliederung

Regeln:
- linke bzw. Hauptspalte für Auswahl / Liste / Vergleich
- rechte Spalte für Details / Empfehlungen / Metriken / Aktionen
- Spalten ausgewogen, kein leerer Totraum

---

## 5. Daten- und Technikkomponenten

### 5.1 Technical Table / List
Zweck:
- strukturierte technische Datensätze

Regeln:
- klar rasterbasiert
- helle Flächen
- zurückhaltende Aktionen
- keine überdekorierte Tabelle

### 5.2 Metric Tile
Zweck:
- einzelne Kennzahl oder kompakte Statuszahl

Regeln:
- knapp
- schnell scannbar
- häufig in Reihen oder kleinen Grids

### 5.3 Inspector Detail Block
Zweck:
- ausgewählte technische Entität im Detail zeigen

Verwendung:
- Endpoint Explorer
- Capture Inspector
- OpenAPI Export
- Schema Drift Empfehlungen / Seitendetails

### 5.4 Version / Delta Strip
Zweck:
- Vergleichszustände zwischen Baseline, aktueller Version und früheren Snapshots

Verwendung:
- Schema Drift

Regeln:
- kompakte horizontale Karten
- klare Statusmarkierung
- Zeitbezug klein und sekundär

### 5.5 Change Item / Drift Row
Zweck:
- einzelne Änderung als technische Zeile darstellen

Bestandteile:
- Method-Tag
- Pfad
- Meta-Information
- Risikostatus
- Aktion / Drill-in

Verwendung:
- Schema Drift

---

## 6. Code- und Snippet-Komponente

### 6.1 Technical Snippet / Codeblock
Status:
- verbindlich verankert, auch wenn nicht überall sichtbar

Mögliche Selektoren:
- `.therapi-codeblock`
- `.code-block`
- `[data-codeblock]`
- `[data-ui="codeblock"]`
- `.api-code-snippet`
- `.capture-fragment`

Pflichtstil:
- **helle** Surface
- neutraler technischer Charakter
- dunkler Text
- Monospace
- Radius im Bereich `10–12px`
- Padding im Bereich `1rem–1.25rem`
- keine dunkle Pflicht-Variante

Praktische Referenzwerte:
- Hintergrund etwa `#F1F5F9`
- Text etwa `#202426`

### 6.2 Copy Button
Selektoren:
- `.therapi-codeblock__copy`
- `.code-block__copy`
- `[data-codeblock-copy]`

Regeln:
- oben rechts
- low emphasis
- hell oder neutral integriert
- nie als primärer CTA behandeln

---

## 7. Seitentypen im Prototyp

### 7.1 Control Panel
Charakter:
- Übersichtsseite
- Status, Metriken, Systemkontext

### 7.2 Endpoint Explorer
Charakter:
- explorativ
- Listen-/Detail-Logik
- technische Inspektionsfläche

### 7.3 Schema Drift
Charakter:
- Vergleich und Änderungsanalyse
- Versionen, Delta-Zustände, Risikobewertung
- linke Hauptinhalte + rechte Metrik-/Empfehlungsspalte

### 7.4 Collections Export
Charakter:
- kuratieren
- bündeln
- Auswahl + Export-Details

### 7.5 Capture Inspector
Charakter:
- technische Request-/Response-Inspektion
- dichter Detailfokus

### 7.6 OpenAPI Export
Charakter:
- Review / Validierung / Export-Paketierung

### 7.7 Settings
Charakter:
- globale Konfiguration
- systemnahe Einstellungsgruppen

---

## 8. Regeln für Wiederverwendung

Ein neues UI-Element soll immer zuerst einer dieser Kategorien zugeordnet werden:

1. Shell
2. Navigation
3. Status
4. Card/Panel
5. Data/Inspector
6. Code/Snippet

Falls es in keine Kategorie passt, darf es **nicht automatisch neu erfunden** werden.  
Dann ist zuerst eine Spezifikations-Erweiterung nötig.

---

## 9. Komponenten-Mapping für künftige KI

Für neue Seiten gilt dieses Minimalset als Pflicht:

- Sidebar
- Topbar
- Page Header
- mindestens ein Standard Card / Panel Muster
- bei technischem Output optional ein heller Technical Snippet / Codeblock

Für explorerartige Seiten zusätzlich:
- Split Layout
- Detail Block
- technische Listen-/Tabellenfläche

Für Analyse-/Drift-Seiten zusätzlich:
- Version / Delta Strip
- Change Rows
- Metrik-Karten
- Empfehlungspanel

Für Einstellungsseiten zusätzlich:
- gruppierte Standard Cards
- klare Abschnittsüberschriften
- keine lockeren Freiflächen
