# Juwelier Krebber — Website

Statische One-Page-Website für Juwelier Krebber, Limitenstraße 55, 41236 Mönchengladbach-Rheydt.
Kein Build-Schritt, keine Abhängigkeiten — `index.html` öffnen genügt.

## Inhalt

```
index.html          fertige Seite (HTML + CSS + Vanilla JS, alles inline)
assets/img/         alle Bilder, lokal eingebunden
source/             ursprüngliche Komponentendateien (.dc.html + support.js)
```

## Aufbau der Seite

01 Das Haus · 02 Uhren (Drag-Slider + Marken-Marquee) · 03 Schmuck · 04 Werkstatt & Service
(Liste mit Bildvorschau am Cursor) · 05 Trauringe · 06 Kontakt

Interaktion: fixierter Header, der beim Runterscrollen einfährt und ab dem Hero hell wird,
Burger-Menü unter 980 px, Scroll-Reveals per IntersectionObserver, Parallax auf Hero- und
Trauringbild. Alle Bewegungen respektieren `prefers-reduced-motion`.

## Anpassen

* **Akzentfarbe / Tempo:** oben im `<script>`-Block, Objekt `PROPS`
  (`accent`, `motion: "Voll" | "Reduziert"`, `marqueeSpeed` in Sekunden).
* **Marken, Services, Kollektionen:** direkt im Markup — es gibt keine Template-Schicht mehr.

## Bilder

Produkt- und Ladenfotos stammen von juwelierkrebber.de und sind lokal abgelegt, damit die Seite
unabhängig vom Shop-CDN läuft. Drei Service-Zeilen hatten keine passenden Motive; dort stehen
Stockfotos von [Unsplash](https://unsplash.com) (Unsplash-Lizenz):

| Datei | Motiv | Quelle |
|---|---|---|
| `service-uhrmacher.jpg` | Uhrwerk in Arbeit | unsplash.com/photos/… `photo-1649803091689-0e65c4e9581f` |
| `service-goldschmiede.jpg` | Löten an der Goldschmiedebank | `photo-1598724168411-9ba1e003a7fe` |
| `service-wertermittlung.jpg` | Edelstein mit Pinzette und Gemmologenlampe | `photo-1705575567619-c9774a05852d` |

## Hinweis

Dies ist ein Entwurf / eine Demo-Umsetzung, nicht die offizielle Website des Unternehmens.
Die offizielle Seite ist [juwelierkrebber.de](https://www.juwelierkrebber.de).
Impressum und Datenschutz sind noch nicht hinterlegt — die Footer-Links verweisen vorerst auf
den Kontaktabschnitt. Vor einem echten Livegang müssen beide Seiten ergänzt werden.
