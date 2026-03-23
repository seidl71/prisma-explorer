# 🔷 PrismaExplorer

**Interaktive 3D-Geometrie-Lernapp für gerade Prismen**
Entwickelt für Jonas (Klasse 8) zum Vertiefen des Verständnisses von geraden Prismen.

---

## 📐 Was die App kann

- **6 Körper** interaktiv erkunden: Würfel, Quader, Quadratisches Prisma, Dreieck-Prisma, Trapez-Prisma und Pyramide
- **3D-Ansicht** mit Maus drehen, mit Scrollrad zoomen
- **Schieberegler** für alle Maße (a, b, h, …) – Formeln und 3D-Modell aktualisieren sich in Echtzeit
- **Bemaßungen** direkt im 3D-Diagramm (gestrichelte Maßlinien mit Tick-Marken und farbigen Labels)
- **Volumen und Oberfläche** mit Formel, berechnetem Ergebnis und Schritt-für-Schritt-Rechnung
- **Pythagoreischer Lehrsatz** – zeigt pro Körper, wo und wie der PLS konkret angewendet wird

---

## 🚀 Verwendung

Keine Installation, kein Build-Tool nötig – einfach die Datei öffnen:

```
prisma-explorer.html   →   doppelklicken oder im Browser öffnen
```

Die App lädt Three.js automatisch über CDN (Internetverbindung erforderlich).
Offline-Nutzung: Three.js-Skript lokal speichern und den CDN-Link in der HTML anpassen.

---

## 🔷 Abgedeckte Körper

| Körper | Parameter | Besonderheit |
|---|---|---|
| Würfel | a | Flächen- und Raumdiagonale mit PLS |
| Quader | l, b, h | Raumdiagonale in 2 PLS-Schritten |
| Quadratisches Prisma | a, h | Grundflächen- und Raumdiagonale |
| Dreieck-Prisma | a, h | Dreieckshöhe mit PLS berechnen |
| Trapez-Prisma | a, c, ht, h | Schenkel des Trapezes mit PLS |
| Pyramide | a, h | Apothema und Seitenkante mit PLS |

---

## 📁 Projektstruktur

```
prisma-explorer.html    ← gesamte App (HTML + CSS + JavaScript, alles in einer Datei)
README.md               ← diese Datei
```

---

## 🛠️ Weiterentwicklung

Mögliche Erweiterungen:
- Weitere Körper (z. B. Zylinder, Kegel, Kugel)
- Aufgabenmodus mit Eingabefeldern und Lösung
- Druckansicht / Export als PDF
- Offline-Modus (Three.js lokal einbetten)
- Mehrsprachige Unterstützung

Die gesamte Logik liegt in `prisma-explorer.html`. Die wichtigsten Abschnitte im JavaScript sind kommentiert mit:
- `GEOMETRY CREATORS` – Three.js Geometrien für jeden Körper
- `SHAPE DEFINITIONS` – Formeln, Beschriftungen und Bemaßungen pro Körper
- `THREE.JS SETUP` – Szene, Kamera, Beleuchtung, Interaktion
- `UI` – Tabs, Schieberegler, Formelanzeige

---

## 📚 Lehrplanbezug

Mathematik, Klasse 8 – Stereometrie: Gerade Prismen
Inhalte: Oberfläche, Volumen, Anwendung des Pythagoreischen Lehrsatzes
