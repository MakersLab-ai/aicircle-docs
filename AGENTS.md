# Handbuch — Anleitungen für KI-Coding-Assistenten

## Was dieses Projekt ist

- Mintlify-Doku unter [handbuch.makerslab.ai](https://handbuch.makerslab.ai) (Custom-Domain folgt nach Live-Schaltung)
- Inhalt: Ersteinrichtung, API-Keys, Telegram-Bot, Preisvergleich
- Zielgruppe: **Endnutzer ohne technischen Hintergrund**
- Sprache: Deutsch (Du-Form)
- Konfiguration: `docs.json`. Vorschau lokal mit `mint dev`, Linkcheck mit `mint broken-links`
- Hinweis: Mintlify-CLI braucht Node ≤ 22 LTS (nicht Node 25+)

## Terminologie (verbindlich)

- **„Agent"** für das, was die Nutzer von uns bekommen. **Nicht** „AI Circle", „Assistent", „Bot" als Produktbezeichnung.
- **„Bot-Token"** für das Telegram-Geheimnis. Nicht „HTTP API Token" (auch wenn BotFather das so labelt — der Begriff darf maximal in Klammern als Wiedererkennungs-Hinweis stehen).
- **„API-Key"** für die KI-Anbieter-Schlüssel.
- **„kostenloses Kontingent"** statt „Free-Tier".
- **Domain**: immer `makerslab.ai`, **nicht** `aimakerslab.de`.

## Tonalität & Stil

- Du-Form, kurze Sätze, eine Idee pro Satz
- Sentence-case für Überschriften
- UI-Elemente fett: **Settings**, **Create Key**
- Code-Formatierung für Dateinamen, Befehle, Pfade, Tokens
- Mehrfach-Anweisungen als Listen oder `<Steps>`, nicht als Fließtext-Aufzählung

## Was hier NICHT auftauchen darf

- Entwickler-/IT-Pro-Vokabular: Git, GitHub, `.env`, Repository, Deploy, Vertex AI ohne Erklärung, Production/Region/Enterprise
- Interne Details aus dem umgebenden Repo: Admin-Agent, Fleet, OpenClaw, Templates, Migrations, SSH, Infrastruktur
- URL des Anmeldeformulars für Bot-Token/API-Keys (Nutzer bekommen den Link individuell von uns)
- Konkrete Pfade auf der Serverseite (`.env`-Dateien, Container, etc.)

## Was im Handbuch fokussiert werden soll

- Was der Nutzer **selbst** tut: Konto anlegen, Token kopieren, ins Anmeldeformular eintragen
- Was der Nutzer **wissen** muss: Kosten, Sicherheit, Limits setzen, Fehlerbehebung

## Workflow-Konventionen

- Bei jeder Änderung an MDX-Inhalt: `mint broken-links` ausführen, bevor du fertig meldest
- ASCII-Anführungszeichen `"` innerhalb von MDX-Attributen (z. B. `<Frame caption="…">`) brechen den Parser. Inneren Anführungszeichen entweder typografisch (`„…"`) setzen oder ganz umformulieren.
- Keine Screenshot-Platzhalter im veröffentlichten Stand (frühere `<Frame caption="Screenshot folgt: …">`-Blöcke wurden bewusst entfernt)
