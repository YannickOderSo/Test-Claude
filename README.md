# Animationen in Code

## 1. Crazy Gambler – Hakari-Dance (`crazy-gambler/index.html`)

Der Crazy Gambler aus **Anime Jackpot** als 3D-Roblox-Figur (three.js). Er tanzt in einer Casino-Kulisse einen Tanz, der von Hakaris Jackpot-Tanz aus Jujutsu Kaisen inspiriert ist. Ein Durchlauf dauert 32 Schläge (128 BPM, ca. 15 Sekunden):

1. **Groove** (Schlag 0–15): Gewicht von Seite zu Seite, federnde Knie, lockere Arme, das freie Bein tippt an
2. **Twist** (Schlag 16–23): tiefe Knie, Füße drehen gegen die Hüfte, Hände rollen umeinander. Dabei zieht er den Hebel, und die Walzen auf der Brust drehen sich.
3. **Jackpot** (Schlag 24–31): Die Walzen landen auf 7-7-7. Er zeigt nach oben, dann gehen beide Arme hoch zum Schulter-Shimmy. Dazu gibt es Münzregen, eine Aura und den JACKPOT-Schriftzug.

**Öffnen:** `crazy-gambler/index.html` doppelklicken. Du brauchst eine Internetverbindung, weil three.js von einem CDN geladen wird.

| Aktion | Wirkung |
| --- | --- |
| Maus ziehen / wischen | Kamera drehen |
| Scrollen / Pinch | Zoom |
| „♪ Musik an“ oder `M` | Eigener Beat, synchron zum Tanz |
| „Pause“ oder Leertaste | Anhalten |

Zum Anpassen: Das `CONFIG`-Objekt enthält Tempo, Neon-Leuchten, Konfetti- und Münzmenge. Die Tanzschritte stehen in den Funktionen `poseGroove`, `poseTwist` und `poseJackpot`; jede Zahl dort ist ein Gelenkwinkel.

## 2. Galaxie (`index.html`)

Eine rotierende Spiralgalaxie aus mehreren tausend leuchtenden Partikeln, gezeichnet mit HTML5 Canvas und reinem JavaScript. Du brauchst keine Installation und keine Bibliotheken.

### Starten

`index.html` doppelklicken, dann öffnet sie sich im Browser.

### Steuerung

| Aktion | Wirkung |
| --- | --- |
| Maus bewegen / wischen | Sterne weichen aus und verwirbeln, danach federn sie zurück |
| Klicken / tippen | Schockwelle mit Funkenregen |
| Leertaste | Pause |
| `N` oder Button „Neue Galaxie“ | Zufällige neue Galaxie (Armzahl, Drehung, Farben) |

Zwischendurch zünden von selbst kleine Supernovae in den Spiralarmen.

### Anpassen

Ganz oben im `<script>`-Teil von `index.html` steht ein `CONFIG`-Objekt. Dort kannst du zum Beispiel ändern:

- `arms`: Anzahl der Spiralarme
- `density`: Partikelmenge
- `rotationSpeed`: Drehgeschwindigkeit
- `innerHue` / `outerHue`: Farben im Kern und am Rand (Farbkreis 0–360)
- `trail`: Länge der Leuchtspuren (kleiner = länger)
- `mouseRadius`: Wirkungsradius der Maus

Datei speichern, Browser neu laden, fertig.
