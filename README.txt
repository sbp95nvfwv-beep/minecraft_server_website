# Minecraft-Server-Website

## Inhalt
- `index.html` – die Website
- `config.js` – Servername, IP, Port und Beschreibung
- `.github/workflows/deploy.yml` – veröffentlicht die Website automatisch mit GitHub Pages

## 1. Vor dem Hochladen anpassen
Öffne `config.js` und ändere mindestens:
- `title`: Name deines Servers
- `ip`: deine Minecraft-/Aternos-Adresse (ohne `https://`)
- `port`: dein Port
- `description`: deine Serverbeschreibung

Speichere die Datei. Die Beispieldaten sind Platzhalter, weil deine echte IP und dein Port noch nicht mitgeteilt wurden.

## 2. Auf GitHub hochladen
1. Entpacke die ZIP-Datei.
2. Erstelle auf GitHub ein neues Repository, z. B. `minecraft-server-website`.
3. Lade **alle Inhalte** des entpackten Ordners in das Hauptverzeichnis des Repositorys hoch. Wichtig: Auch den versteckten Ordner `.github` samt `workflows/deploy.yml` hochladen.
4. Öffne im Repository **Settings → Pages**.
5. Bei **Build and deployment → Source** wählst du **GitHub Actions**.
6. Warte, bis der Workflow unter dem Reiter **Actions** grün abgeschlossen ist.
7. Unter **Settings → Pages** wird deine öffentliche Website-Adresse angezeigt.

Bei jedem späteren Push/Upload auf den Branch `main` wird die Website automatisch neu veröffentlicht. Du kannst den Workflow außerdem im Reiter **Actions** manuell starten.

## 3. Was die Website kann
- IP und Port kopieren
- Online-/Offline-Status über den externen Dienst `mcsrvstat.us` abfragen (ungefähr jede Minute)
- Serverbeschreibung anzeigen
- Kommentare und 👍/👎-Bewertungen im Browser speichern

## Wichtige Grenzen
GitHub Pages hostet nur statische Dateien. Kommentare und Bewertungen werden in dieser Version nur im Browser des jeweiligen Besuchers gespeichert und nicht mit anderen Besuchern geteilt. Für gemeinsame Kommentare/Bewertungen braucht die Website einen zusätzlichen Dienst oder ein Backend (z. B. Giscus für Kommentare über GitHub Discussions).

Der Admin-Bereich ist nur eine einfache lokale Bearbeitungshilfe. Das Passwort steht öffentlich in `config.js` und ist daher **kein sicherer Schutz**. Änderungen dort werden nur im eigenen Browser gespeichert. Für dauerhaft sichtbare Änderungen bearbeitest du `config.js` und lädst die Datei erneut zu GitHub hoch.

Deine echte Server-IP, dein Port und dein gewünschter Servername fehlen noch. Deshalb ist die Website vorbereitet, aber noch nicht mit deinen persönlichen Serverdaten befüllt.
