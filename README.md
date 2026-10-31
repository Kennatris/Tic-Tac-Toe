# Tic-Tac-Toe auf dem Arduino

**Arduino Uno · C++ · FastLED · Hardwareprojekt / 2026**

Ein Tic-Tac-Toe-Spiel zum Anfassen: Neun Taster bilden das Spielfeld, farbige LEDs zeigen die Züge. Gespielt wird zu zweit oder gegen einen Minimax-Gegner. Ein Drehregler verändert dessen Fehlerwahrscheinlichkeit.

![Schematischer Aufbau mit Tastern, Arduino und LEDs](docs/media/aufbau.svg)

[Projekt und Technik](docs/PROJEKT.md) · [LED-Muster](docs/GALERIE.md) · [Quellcode herunterladen](https://github.com/Kennatris/Tic-Tac-Toe/archive/refs/heads/main.zip)

## Spielumfang

- Zwei-Spieler-Modus und Computergegner mit Minimax und Alpha-Beta-Beschneidung.
- Einstellbare Fehlerwahrscheinlichkeit über ein Potentiometer.
- Startanimation, blinkende Gewinnreihe und Unentschiedenanimation.
- Eigene Status-LED für Spielmodus und aktiven Demo-Spieler.
- Automatischer Demomodus nach 60 Sekunden ohne Eingabe.
- Neustart über einen eigenen Taster.

![Start-, Gewinn- und Unentschiedenmuster der Firmware](docs/media/spielzustaende.svg)

## Bedienung

1. Am Modusschalter zwischen Computer und Mitspieler wählen.
2. Für den Computergegner die Schwierigkeit am Drehregler einstellen.
3. Einen Spielfeldtaster drücken, um einen Zug zu setzen.
4. Mit dem Reset-Taster eine neue Runde beginnen.

Die Abbildungen zeigen die Pinzuordnung und LED-Muster schematisch nach der Firmware. [Aufbau und Start mit der Arduino IDE](docs/PROJEKT.md#aufbau-und-start).

> **Hinweis:** Dokumentation und Zusammenfassung wurden automatisiert durch einen Agenten erstellt und dienen der Veranschaulichung. Der Programmcode ist unverändert. Alle Angaben und Downloads ohne Gewähr.
