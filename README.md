# System Position (RAW)

Dieses Modul liefert neutrale Positionsdaten für das System.
Keine Logik. Keine Engine. Keine Interpretation.

## Position
- pos12: 0–11        (12‑Raum)
- pos4: 0–3          (4‑Achsen‑Band)
- vpos: 0–3          (virtuelle Achse)

## Nähe
- next12: (pos12+1)%12
- prev12: (pos12+11)%12
- next4:  (pos4+1)%4
- prev4:  (pos4+3)%4
- nextV:  (vpos+1)%4
- prevV:  (vpos+3)%4

## Zweck
Diese Werte dienen ausschließlich der Orientierung für andere Module
(OS, CALC, LIVE, NC, Operatoren).

## Verhalten
Dieses Modul führt keine Logik aus.
Es bewegt nichts.
Es entscheidet nichts.
Es interpretiert nichts.

## Nutzung
Die Positionswerte können direkt ausgelesen und weiterverarbeitet werden.
Alle Achsen (12‑Raum, 4‑Band, virtuelle Achse) bleiben stabil und neutral.

## Status
RAW‑Material. Schnittstellen‑fähig. EVO‑kompatibel.
