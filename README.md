# Kugellabyrinth

Ein 3D-Kugelspiel, das direkt im Browser läuft – ohne Installation, auf PC und Handy.

## Spielmodi

**Sphäre (30 Level)**
Eine Glaskugel mit Bahnen im Inneren: Spiralen, Treppen, Wellen und schmale Stege. Kipp und dreh die Kugel, bis die Stahlkugel von S bis Z rollt. Nummerierte Etappen sind Rücksetzpunkte.

**Holzplatte (100 Level)**
Klassisches Labyrinth mit Löchern. Neig die Platte und roll die Kugel vom goldenen Ring ins grüne Loch. Fällt sie durch, beginnt das Level von vorn.

## Steuerung

| | Sphäre | Holzplatte |
|---|---|---|
| Maus / Finger ziehen | Kugel kippen | Platte neigen |
| Rechte Maustaste / `Q` `E` | Kugel drehen | – |
| Pfeiltasten / `WASD` | kippen | neigen |
| `Shift` | feiner | feiner |
| Mausrad | zoomen | zoomen |
| `R` / `Esc` / `M` | Neustart / Pause / Ton | Neustart / Pause / Ton |

Die Maus-Empfindlichkeit lässt sich in den Einstellungen für beide Modi getrennt einstellen. Fortschritt und Bestzeiten speichert der Browser.

## Technik

Eine einzige Datei (`index.html`) mit [three.js](https://threejs.org/) 0.160 für die 3D-Grafik. Die Physik (rollende Kugel, Kollisionen, Löcher) ist selbst geschrieben, die Level werden aus festen Startwerten erzeugt und sehen deshalb bei jedem Start gleich aus.

Lokal starten: `index.html` über einen beliebigen Webserver öffnen, z. B.

```
python -m http.server 8000
```

und dann http://localhost:8000 aufrufen.
