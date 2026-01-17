# Research

This is my own research using (mostly) my phone (using NFC Tools). Credits also go to [@anonymos3584](https://github.com/anonymos3584) for helping me with the identification and research deep dive.

## 17.01.2026 - DB Regio RB (Baden Württemberg)

Method: Raw reading

Raw NFC data read from the tag: `2026-01-17-RB.nfc` (file)

Tag location: Toilet lamp on the bottom (marked with an NFC symbol)

Reading: `DB.FZ.1;94800440027-1;94800441027-0;WC1;#`

Wagon identifier: `94 80 0441027-0 D-DB`
![](IMG_20260117_183819747.png)

### String decoding

```
DB.FZ.1;94800440027-1;94800441027-0;WC1;#
 |  |  |     |               |        |
 |  |  |     |               |       Tag location
 |  |  |     |               |
 |  |  |     |               |
 |  |  |     |            Wagon identifier (94800441027-0)
 |  |  |     |
 |  |  | Likely train identifier
 |  | Indentifier version (?)
 | Likely the shortening of "Fahrzeug" or vehicle in German
Provider
```
