\# TicTacToe for Educational Purposes



\*\*Author:\*\* Tino J. Strasser  

\*\*Date:\*\* January 22, 2026  

\*\*Platform:\*\* Arduino Uno / FastLED



---



\## English Documentation



\### Overview

This project is an educational implementation of the classic Tic-Tac-Toe game using an Arduino Uno and WS2812B LEDs (Neopixel). It is designed to teach students hardware abstraction, game logic, and state management. The game features a smart AI opponent (Minimax algorithm) with adjustable difficulty and a 2-player mode.



\### Hardware Setup \& Pinout



| Component | Pin / Port | Description |

| :--- | :--- | :--- |

| \*\*Game Grid (Buttons)\*\* | D2, D3, D4 | Top Row (Left to Right) |

| | D7, D8, D9 | Middle Row (Left to Right) |

| | D10, D11, D12 | Bottom Row (Left to Right) |

| \*\*LED Grid\*\* | D6 | Strip with 9 WS2812B LEDs (Game Board) |

| \*\*Status LED\*\* | D5 | Single WS2812B LED (Status Indicator) |

| \*\*Difficulty Control\*\* | A0 | Potentiometer (0% - 100% AI Error Rate) |

| \*\*Mode Switch\*\* | A1 | Switch (LOW = Computer, HIGH = 2-Player) |

| \*\*Reset Button\*\* | A2 | Button (Active LOW) |



\### LED Status Indicators (Pin D5)

The single status LED on Pin D5 provides visual feedback on the current game state:

\* \*\*Red / Blue Blinking:\*\* System Boot / Reset in progress.

\* \*\*Green:\*\* Playing against Computer (AI Mode).

\* \*\*Yellow:\*\* Playing against Human (2-Player Mode).

\* \*\*Red / Blue (Solid):\*\* In Idle Mode, shows the active player of the demo game.



\### How to Play

1\.  \*\*Select Mode:\*\* Use the switch on \*\*A1\*\* to choose between playing against the computer or another player.

2\.  \*\*Set Difficulty:\*\* If playing against the computer, turn the potentiometer on \*\*A0\*\*.

&nbsp;   \* \*0% (Min):\* Perfect AI (Minimax). Impossible to beat.

&nbsp;   \* \*100% (Max):\* The AI makes random mistakes often.

3\.  \*\*Start Game:\*\* Press any grid button to place your mark (Color depends on player).

4\.  \*\*Reset:\*\* Press the button on \*\*A2\*\* to restart the game at any time.



---



\## Deutsche Dokumentation



\### Überblick

Dieses Projekt ist eine pädagogische Umsetzung des klassischen Tic-Tac-Toe-Spiels unter Verwendung eines Arduino Uno und WS2812B-LEDs (Neopixel). Es wurde entwickelt, um Schülern Hardware-Abstraktion, Spielelogik und Zustandsverwaltung beizubringen. Das Spiel verfügt über einen intelligenten KI-Gegner (Minimax-Algorithmus) mit einstellbarem Schwierigkeitsgrad sowie einen 2-Spieler-Modus.



\### Hardware-Aufbau \& Pin-Belegung



| Komponente | Pin / Port | Beschreibung |

| :--- | :--- | :--- |

| \*\*Spielfeld (Taster)\*\* | D2, D3, D4 | Obere Reihe (Links nach Rechts) |

| | D7, D8, D9 | Mittlere Reihe (Links nach Rechts) |

| | D10, D11, D12 | Untere Reihe (Links nach Rechts) |

| \*\*LED Raster\*\* | D6 | Strip mit 9 WS2812B LEDs (Spielfeld) |

| \*\*Status LED\*\* | D5 | Einzelne WS2812B LED (Statusanzeige) |

| \*\*Schwierigkeit\*\* | A0 | Potentiometer (0% - 100% KI-Fehlerrate) |

| \*\*Modus-Schalter\*\* | A1 | Kippschalter (LOW = Computer, HIGH = 2-Spieler) |

| \*\*Reset Taster\*\* | A2 | Taster (Active LOW) |



\### LED Status-Anzeigen (Pin D5)

Die einzelne Status-LED an Pin D5 gibt visuelles Feedback über den aktuellen Spielstatus:

\* \*\*Rot / Blau Blinkend:\*\* Systemstart / Reset wird ausgeführt.

\* \*\*Grün:\*\* Spiel gegen den Computer (KI-Modus).

\* \*\*Gelb:\*\* Spiel gegen einen Mitspieler (2-Spieler-Modus).

\* \*\*Rot / Blau (Dauerhaft):\*\* Im Idle-Modus (Ruhemodus) zeigt sie den aktiven Spieler des Demo-Spiels an.



\### Spielanleitung

1\.  \*\*Modus wählen:\*\* Nutze den Schalter an \*\*A1\*\*, um zwischen "Gegen Computer" und "Gegen Mitspieler" zu wählen.

2\.  \*\*Schwierigkeit einstellen:\*\* Wenn du gegen den Computer spielst, drehe am Potentiometer an \*\*A0\*\*.

&nbsp;   \* \*0% (Min):\* Perfekte KI (Minimax). Unmöglich zu besiegen.

&nbsp;   \* \*100% (Max):\* Die KI macht häufig zufällige Fehler.

3\.  \*\*Spiel starten:\*\* Drücke einen Taster auf dem Spielfeld, um dein Zeichen zu setzen.

4\.  \*\*Neustart:\*\* Drücke jederzeit den Taster an \*\*A2\*\*, um das Spiel neu zu starten.

