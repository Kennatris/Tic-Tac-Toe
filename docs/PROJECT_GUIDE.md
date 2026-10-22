# Arduino Tic-Tac-Toe: Projektleitfaden

[Einstieg](../README.md) · [Agentenregeln](../AGENTS.md) · Inventarstand 22.10.2026.

## Zweck und vorhandener Stand

Lehrprojekt für Arduino Uno, FastLED und ein LED-/Taster-Spielfeld mit vorhandener zweisprachiger Hardwaredokumentation.

Geprüfter Branch: `main`; Ausgangscommit `7f9183411e9fcdfb81e824dc9f94f6f6d340485f`. Die folgende Struktur stammt aus dem vorhandenen Git-Baum, nicht aus einer behaupteten erfolgreichen Installation.

## Aufbau und Einstieg

- [tic_tac_toe_solution_v1.ino](../tic_tac_toe_solution_v1.ino)

Weitere vorhandene Hauptbereiche: `README.md`, `TicTacToe.cpp`, `TicTacToe.h`, `tic_tac_toe_solution_v1.ino`.

## Einrichtung und Prüfungen

Zuerst die vorhandenen Projekt-/Paketdateien und Agentenregeln lesen. Verfügbare Toolchain und Versionen vor Installation feststellen. Nur vorhandene Manifeste/Lockfiles verwenden; keine Abhängigkeiten aus dem Projektnamen erfinden.

```bash
python3 .github/scripts/check-project-docs.py
```

Das Dokumentationsgate arbeitet ohne Anwendungsausführung oder externe APIs. Weitere aufgeführte Befehle sind aus dem Projekt abgeleitete nächste Prüfungen; ihr erfolgreicher Lauf auf der Zielumgebung wird durch diesen Leitfaden nicht behauptet. Bei geräte-, GUI-, Broker- oder Datenbankabhängigen Prüfungen gelten die folgenden Grenzen.

## Daten, Betrieb und Sicherheit

Pinbelegung und Hardwareannahmen mit README abgleichen. Kein Flashen, keine Port-/Gerätezugriffe ohne konkreten Geräteauftrag. Spielregeln, Zugvalidierung und Minimax getrennt von der Hardware prüfen.

Konfigurationen, Datenquellen, erzeugte Artefakte und ihre Aufbewahrung dokumentieren. Produktiv-/Nutzerdaten haben eine getrennte Sicherung und einen geprüften Rückweg. Keine Cloudübertragung, Kosten, Releases oder Deployments als Nebenwirkung eines Dokumentationstests.

## Änderungen und Abnahme

[Beitragsablauf](../CONTRIBUTING.md) beschreibt Branch, PR und Tests; [Sicherheitsmeldungen](../SECURITY.md) beschreibt den vertraulichen Meldeweg. Änderungen an Schnittstellen, Datenformaten oder Betrieb aktualisieren die Dokumentation im selben Change. Kleine nachvollziehbare Änderungen und ein datenkompatibler Rückweg gehören bei relevanten Eingriffen zur Abnahme.

## Lizenz und Herkunft

Im geprüften Baum wurde keine eigenständige Lizenzdatei nachgewiesen. Vor externer Wiederverwendung Rechte und Lizenz mit den Rechteinhabern klären; dieser Change wählt keine neue Lizenz.

## Offene Nachweise

- Branchschutz aktuell nicht als aktiv gemeldet; konkrete Regeln, Secret Scanning, Push Protection und Code Scanning wurden mit diesem Dokumentationschange nicht als vollständig eingerichtet nachgewiesen.
