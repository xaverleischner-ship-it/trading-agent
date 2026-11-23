# Trading Agent Free – Android/PWA

## Was diese Version kann
- Kostenloses statisches Webprojekt ohne Server, Backend, API-Schlüssel oder Abo.
- Installierbare PWA auf Android über HTTPS.
- Lokale technische Auswertung (SMA-Trend, Momentum, MACD-ähnliche EMA-Differenz, RSI) für Gold, Nasdaq 100 und TTWO.
- Import historischer OHLC-CSV-Daten; Signaljournal bleibt im Browser-Speicher des Geräts.
- Externe Chartlinks zu TradingView.

## Ehrliche Grenzen
Diese Version lädt KEINE Kurse automatisch und bietet KEINE vier trainierten ML-Modelle. Sie erzeugt kein Signal, solange keine CSV-Kursdaten importiert wurden. Der aktuelle Kurs wird nicht verwendet, wenn keine passende Historie importiert wurde. Technische Regeln sind heuristisch, nicht validiert und keine Gewinnwahrscheinlichkeiten. Für zuverlässige automatische Live-Daten wäre ein Datenanbieter/Backend erforderlich; vollständig kostenlose und zuverlässige Echtzeitdaten sind nicht garantiert.

## Kostenlos online stellen (GitHub Pages)
1. GitHub-Konto öffnen und neues **Public** Repository anlegen, z. B. `trading-agent-free`.
2. Den Inhalt dieses Ordners (index.html, app.js, style.css, manifest.webmanifest, sw.js, Icons) in das Repository-Hauptverzeichnis hochladen. Nicht den übergeordneten Ordner als einzigen Ordner hochladen.
3. Repository → Settings → Pages.
4. Bei Build and deployment `Deploy from a branch` wählen, Branch `main`, Ordner `/ (root)`, Save.
5. Warten, bis GitHub Pages eine `https://...github.io/...` Adresse anzeigt.
6. Adresse auf Samsung in Chrome öffnen → ⋮ → „App installieren“/„Zum Startbildschirm hinzufügen“.

GitHub Pages ist kostenlos für öffentliche Repositories. Der Quellcode ist damit öffentlich sichtbar. Keine Passwörter oder privaten Daten in die Dateien schreiben.

## CSV Format
Mindestens 40 Zeilen, älteste zuerst. Kopfzeile mit Date, Open, High, Low, Close (Volume optional), Trennzeichen Komma, Semikolon oder Tab. Dezimalwerte mit Punkt oder Komma (bei CSV mit Komma als Trennzeichen besser Punkt verwenden).

## Nutzung
1. TradingView-Link öffnen und Marktdaten/Chart prüfen.
2. Historische OHLC-CSV für dasselbe Symbol und den gewünschten Zeitrahmen beschaffen.
3. CSV importieren und „Markt analysieren“ drücken.
4. BUY/SELL/ABWARTEN ist eine regelbasierte technische Einordnung, keine Handelsempfehlung.

Keine Broker-Anbindung, keine automatische Orderausführung, keine Anlageberatung. CFDs können zum vollständigen Verlust des eingesetzten Kapitals führen.
