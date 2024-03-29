# Operation Gazelle

## Namensherkunft

Die Bennenung ist willkürlich. Alles mit Operation klingt geheimnisvoll.

## Ziel des Projektes

Eine funktionierende, intelligente und automatisierte Steuerung der Bewässerung des Gartens.

Dafür werden folgende Bedingungen als eine Art grobes Lastenheft definiert:

- Einzelnes Ansteuern der einzelnen Ventile
- 3+1 Ventile für den Rasen 
- Erweiterungsventile (vorerst nicht in Planung einezogen):
  - 2+1 Ventile für das Hochbeet (Verschiedene Bewässerungsarten der einzelnen Pflanzenarten)
  - 2+1 Ventile für Vorgarten
  - 1+1 Ventil für Sträucher
  - 2+1 Ventile für langes Beet
- Sensoren:
  - Regensensor (digital)
  - Temperatursensor (Redundanz! -> 2?) (analog)
  - Feuchtigkeitssensoren an verschiedenen Stellen (analog) (vorerst nur einen für den Rasen)
  - Sensor zur Füllstandsmessung Zisterne (analog)
- Funktionen:
  - Kein Gießen bei Regen und einer Stunde danach
  - Entwässerung bei T > 5°C (Zwingende, allseits gültige Bedingung)
  - Entwässerung in bestimmten Zeitraum (z.B. Oktober - März)
  - Bewässerung nur in den Abendstunden (Sonnenlicht könnte bei Wassertropfen Lupeneffekt haben)
  - Wechsel zwischen Zisternen- auf Leitungswasserbetrieb bei einem bestimmten Füllstand
  - Wechselnde Bewässerung der einzelnen Rasenabschnitte
  - Ausschalten der Bewässerung für 4 Stunden
  - Dauerhaftes Entwässern (=Ausschalten) der Bewässerung
  - Bewässerung nur bei zu wenig Feuchtigkeit
- Beachten: Erweiterbarkeit!

## Notizen

- Regensensor: Wie lange zeigt der nach dem Regen an, dass es regnet? -> Ausschaltverzögerung gangbar?