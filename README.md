# Galaxie – interaktive Animation

Eine rotierende Spiralgalaxie aus mehreren tausend leuchtenden Partikeln, gezeichnet mit HTML5 Canvas und reinem JavaScript. Du brauchst keine Installation und keine Bibliotheken.

## Starten

`index.html` doppelklicken, dann öffnet sie sich im Browser.

## Steuerung

| Aktion | Wirkung |
| --- | --- |
| Maus bewegen / wischen | Sterne weichen aus und verwirbeln, danach federn sie zurück |
| Klicken / tippen | Schockwelle mit Funkenregen |
| Leertaste | Pause |
| `N` oder Button „Neue Galaxie“ | Zufällige neue Galaxie (Armzahl, Drehung, Farben) |

Zwischendurch zünden von selbst kleine Supernovae in den Spiralarmen.

## Anpassen

Ganz oben im `<script>`-Teil von `index.html` steht ein `CONFIG`-Objekt. Dort kannst du zum Beispiel ändern:

- `arms`: Anzahl der Spiralarme
- `density`: Partikelmenge
- `rotationSpeed`: Drehgeschwindigkeit
- `innerHue` / `outerHue`: Farben im Kern und am Rand (Farbkreis 0–360)
- `trail`: Länge der Leuchtspuren (kleiner = länger)
- `mouseRadius`: Wirkungsradius der Maus

Datei speichern, Browser neu laden, fertig.
