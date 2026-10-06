<!-- ELUCENIA technical documentation · has-bled · de · no clinical/professional/rights approval -->

# HAS-BLED

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/has-bled)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Unkontrollierte Hypertonie (systolischer Blutdruck \> 160 mmHg)

`h`

### Eingeschränkte Nierenfunktion (Dialyse, Transplantation oder Kreatinin ≥ 2,26 mg/dL)

`rim`

### Gestörte Leberfunktion (Zirrhose oder Bilirubin \> 2× und AST/ALT \> 3× des Normalwerts)

`fig`

### Früherer Schlaganfall

`avc`

### Frühere Blutung oder Prädisposition (Anämie, Thrombozytopenie)

`sang`

### Labile INR (Zeit im therapeutischen Bereich \< 60 %)

`inr`

### Alter \> 65 Jahre

`idoso`

### Thrombozytenaggregationshemmer oder Entzündungshemmer

`drogas`

### Alkohol (≥ 8 Getränke pro Woche)

`alcool`

## Fassung der Methode

HAS-BLED/Pisters 2010: 9 Punkte; Niere/Leber/Medikamente/Alkohol getrennt; ESC 2024-Kontext

## Dokumentierte Formel

Je ein Punkt: H Hypertonie, A Nieren-/Leberfunktionsstörung (je 1), S Schlaganfall, B Blutung, L labiler INR, E Alter (\> 65), D Medikamente/Alkohol (je 1). Maximum: 9.

## Grenzen und Population

Der ursprüngliche HAS-BLED schätzt schwere Blutungen innerhalb eines Jahres bei Vorhofflimmern. Die Summe ist keine automatische Kontraindikation zur Antikoagulation; Faktorendefinitionen und aktuelle Empfehlungen müssen zur Version passen. Kalibrierung und antithrombotische Behandlung der Population beeinflussen die Interpretation.

## Referenzen

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Hohes Blutungsrisiko

| Ergebnisdetails | |
| --- | --- |
| Schwere Blutung | 12,50 oder mehr pro 100 Patientenjahre |

Modifizierbare Faktoren: Blutdruck kontrollieren, INR stabilisieren oder auf DOAK umstellen, Thrombozytenaggregationshemmer/NSAR überprüfen, Alkohol reduzieren.


### 2

Hohes Blutungsrisiko

| Ergebnisdetails | |
| --- | --- |
| Schwere Blutung | 3,74 pro 100 Patientenjahre |

Modifizierbare Faktoren: Blutdruck kontrollieren.


### 3

Niedriges Blutungsrisiko

| Ergebnisdetails | |
| --- | --- |
| Schwere Blutung | 1,13 pro 100 Patientenjahre |

