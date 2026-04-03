# THERAPI Prototype — verbindliche Design-Spezifikation

Status: **authoritative working spec derived from the current prototype**  
Scope: **the 7 HTML screens currently bundled in this prototype**

Source-of-truth-Priorität:
1. vorhandene Prototyp-HTML-Dateien
2. diese `DESIGN.md`
3. explizite spätere Amendments
4. alles andere ist **nicht zulässig**

## Zweck

Diese Datei ist absichtlich als **Anti-Spekulations-Spezifikation** formuliert.  
Jede weitere KI, jeder Generator und jede manuelle Umsetzung muss sich **strikt** an diese Vorgabe halten.

**Verboten:**
- Farben frei interpretieren
- Shell, Sidebar, Topbar oder Headline-Position neu erfinden
- zusätzliche Pattern erfinden, die im Prototyp nicht angelegt sind
- Layout „modernisieren“, „optimieren“ oder „vereinfachen“, ohne explizite Freigabe
- aus einzelnen Token-Sets ein neues Master-Design ableiten

**Erlaubt:**
- bestehende Muster exakt replizieren
- vorhandene Komponenten auf weitere Seiten übertragen
- fehlende Inhalte mit bestehenden Komponenten auffüllen
- Responsiveness technisch ergänzen, ohne visuelle Hierarchie zu verändern

---

## Enthaltene Screens

Der aktuelle Prototyp umfasst diese **7** Seiten:

1. `control-panel.html`
2. `endpoint-explorer.html`
3. `schema-drift.html`
4. `capture-inspector.html`
5. `openapi-export.html`
6. `collections-export.html`
7. `settings.html`

Es gibt **keine** zusätzliche kanonische „Collections Export Variant“ im verbindlichen Screen-Set.  
Falls ältere Dateien oder Zwischenstände Varianten enthalten, sind sie **nicht** als neue Seitengattung zu behandeln.

---

## Verbindliche Shell-Regeln

### 1) App-Rahmen
Jede Seite verwendet denselben Grundaufbau:

- `<body>` als horizontaler App-Frame
- linke Sidebar mit fixer Breite
- rechte Hauptfläche als vertikaler Stack
- oben eine Topbar
- darunter der eigentliche Seiteninhalt

### 2) Sidebar
**Verbindlich:**
- Breite: `240px`
- helle Fläche
- Logo oben
- Hauptnavigation vertikal
- Settings unten im separierten Bereich oder als klar abgesetzter Abschluss
- ruhige, kompakte Navigationsdichte

**Nicht ändern:**
- Position links
- vertikale Reihenfolge der Navigation
- visuelle Dominanz der aktiven Seite
- keine zweite Sidebar-Logik
- keine alternative linke Navigation als Pattern-Ersatz

### 3) Topbar
**Verbindlich:**
- Höhe: `56px` (`h-14`)
- oben angeordnete Status-/Kontextgruppe
- helle Fläche mit feiner Unterkante oder sehr dezenter Separation
- kein Hero-Banner
- keine großformatige Suchleiste als Hauptelement, wenn die Seite sie nicht bereits braucht

### 4) Seitenkopf / Headline
**Verbindlich:**
- Headline direkt unter der Topbar im Content-Bereich
- Headline-Stil visuell in der Familie `text-4xl font-extrabold tracking-tight`
- Subline direkt beim Titel, nicht als loser Hero
- keine großen Leerflächen oberhalb des Inhalts

### 5) Content-Prinzip
Der Prototyp bevorzugt:
- dichte Informationsflächen
- Cards und Panels
- 2- bis 3-spaltige Organisation, wenn sinnvoll
- keine riesigen leeren Container
- keine dekorativen Vollbreiten-Heroes

---

## Verbindliche visuelle Leitplanken

### Stabil sichtbare Kernfarben
Diese Werte sind praktisch verbindlich:

- App-Hintergrund: `#F7F9FB`
- Haupttext: `#191C1E`
- aktive Navigations-/Akzentfarbe: `#006B5F`
- helle Panel-/Surface-Töne: `#FFFFFF`, `#F2F4F6`, `#E6E8EA`, `#E0E3E5`
- neutrale Borders: sehr hell, slate-/gray-nah
- Status-/Semantikflächen: ruhig, technisch, nicht bunt

### Wichtige Token-Regel
Im Prototyp existieren mehrere page-lokale Tailwind-Token-Sets. Deshalb gilt:

- **kein** neues globales Farbsystem erfinden
- **kein** freies Neumischen von Blau, Petrol, Mint oder Teal
- für neue Seiten zuerst die sichtbar konsistente Shell-Palette verwenden:
  - Hintergrund `#F7F9FB`
  - aktive Navigation `#006B5F`
  - weiße bzw. sehr helle Cards
  - dunkler Standardtext
- falls eine Seite page-lokale Tokens braucht, müssen diese aus einer existierenden Seite kopiert werden, nicht frei erfunden

---

## Typografie

### Primärschrift
- `Inter`

### Headline
- Größe: visuell `text-4xl`
- Gewicht: `font-extrabold`
- Tracking: `tracking-tight`

### UI-Text
- kompakt
- sachlich
- keine verspielte Typografie
- keine Serifenschrift
- kein übertriebener Gewichtsmix

### Monospace / technische Ausgaben
- UI-Monospace / SFMono / Menlo / Monaco / Consolas / Liberation Mono / Courier New
- ausschließlich für technische Inhalte wie Code, Payloads, Keys oder strukturierte Ausgaben

---

## Radius, Abstände, Dichte

### Radius
Im Prototyp wiederkehrend:
- Navigation / kleine Chips: rund `10px`
- größere Panels / Cards: ungefähr `12px`
- technische Snippets / Codeblöcke: weich gerundet, ebenfalls im Bereich `10–12px`

### Spacing
Verbindliches Dichteprinzip:
- kompakt bis mitteldicht
- keine unnötigen XXL-Abstände
- Cards dürfen Luft haben, aber nicht „schweben“
- Seiten müssen inhaltlich gefüllt wirken, nicht leer

---

## Verbindliche Komponentenregeln

### Navigation Item
- Icon links
- Label rechts
- aktive Seite in Akzentfarbe
- aktive Fläche leicht getönt
- kein starker Schatten

### Status Badge / Topbar Chip
- kleine horizontale Kapsel
- Icon oder Statuspunkt optional
- semantischer Text
- in der Topbar gruppiert

### Card / Panel
- helle Fläche
- weicher Radius
- feine Border oder sehr dezente Trennung
- keine brutalen Schatten
- Inhalt kompakt und funktional

### Tabellen- / Listenflächen
- technisch, klar, sachlich
- helle Hintergründe
- gute Spaltentrennung
- Aktionselemente zurückhaltend

---

## Verbindliche Regel für Codeblöcke / technische Snippets

Auch wenn aktuell nicht auf jeder Seite ein sichtbarer Codeblock vorkommt, ist die **Darstellung technischer Snippets verbindlich im Design verankert**.

### Codeblock-Look
Pflichtcharakter:
- **helle** Surface
- neutraler, ruhiger Technical-Look
- dunkler Text auf heller Fläche
- kein dunkler Night-Surface-Look
- keine neonartige Farbgebung

### Praktische Leitwerte
Diese Werte orientieren sich an den vorhandenen hellen Referenzen und dürfen als Standard verwendet werden:

- Hintergrund: `#F1F5F9` oder ein sehr naher heller Slate-Ton
- Text: `#202426` oder ein sehr dunkler neutraler Grauton
- Border: sehr hell, subtil
- Radius: `10–12px`
- Padding: ca. `1rem` bis `1.25rem`
- Monospace-Schrift
- zurückhaltender, leichter Shadow nur falls im restlichen Screen bereits genutzt

### Copy Button
Falls vorhanden:
- oben rechts im Block
- visuell zurückhaltend
- heller Elevated-Look oder sehr dezente neutrale Fläche
- kein dominanter CTA-Stil

### Harte Regel
Ein zukünftiger Codeblock darf **nicht** als dunkle Pflichtkomponente definiert werden.  
Der verbindliche Stil ist **hell, neutral, technisch und zurückhaltend**.

---

## Verhalten für zukünftige KI-Generierung

Jede weitere KI muss nach diesen Regeln arbeiten:

1. **Erst replizieren, nie interpretieren**
2. Nur Komponenten verwenden, die in dieser Spezifikation oder im Prototyp vorkommen
3. Neue Seiten müssen dieselbe Shell benutzen:
   - Sidebar links
   - Topbar oben
   - Headline unter Topbar
   - kompakte Content-Fläche
4. Technische Snippets/Codeblöcke immer hell und neutral
5. Keine großen Leerflächen
6. Keine neue Farbpalette
7. Keine neue Navigationslogik
8. Keine Hero-Sektion, wenn sie nicht ausdrücklich verlangt wird

---

## Was eine KI tun darf, ohne Rückfrage

- neue Seite in bestehender Shell anlegen
- vorhandene Cards mehrfach verwenden
- bestehende Badge-/Chip-Logik übernehmen
- Tabellen, Listen, Detailpanels im gleichen Stil ergänzen
- technische Snippets im hellen Pflichtstil einsetzen

## Was eine KI nicht tun darf, ohne Rückfrage

- globale Rebrandings
- Sidebar umbauen
- Topbar verschieben oder ersetzen
- Headline-Zone anders anordnen
- Akzentfarbe ändern
- Codeblöcke dunkel uminterpretieren
- neue visuelle Sprache einführen

---

## Definition of done für neue Seiten

Eine neue Seite ist nur dann richtig, wenn sie:

- dieselbe Sidebar verwendet
- dieselbe Topbar verwendet
- denselben Headline-Stil verwendet
- dieselbe Inhaltsdichte wahrt
- keine spekulativen Komponenten enthält
- die bestehende Palette respektiert
- bei Bedarf den hellen technischen Snippet-Stil übernimmt
