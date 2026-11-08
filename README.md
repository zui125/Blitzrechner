# Blitzblick-Training (Punktedetektive)

Lernseite für Kinder: Blitzblick-Training zum Erkennen von Zahlenmengen (0–4, 0–6, 0–10)
mit verschiedenen Bilddarstellungen (Fünfer-/Zehnerfeld, Würfel, Strichliste),
vier Schwierigkeitsstufen (Anzeigedauer 2,0 s bis 0,8 s) und Sternchen-Belohnung.

Reine statische Webseite – eine einzige Datei (`index.html`), keine Abhängigkeiten,
keine Server-Logik. Die „Sterne gesamt" werden lokal im Browser gespeichert (localStorage).

## Lokal öffnen
Einfach `index.html` doppelklicken – fertig.

## Online stellen (GitHub Pages)
1. Auf github.com ein neues **public** Repository anlegen, z. B. `blitzblick-training`.
2. Lokal verbinden und hochladen:
   ```
   git init
   git add .
   git commit -m "Blitzblick-Training: erste Version"
   git branch -M main
   git remote add origin https://github.com/DEIN-BENUTZERNAME/blitzblick-training.git
   git push -u origin main
   ```
3. Im Repo auf GitHub: **Settings → Pages → Source: „Deploy from a branch" → Branch `main`, Ordner `/ (root)` → Save**.
4. Nach ca. 1 Minute ist die Seite erreichbar unter:
   `https://DEIN-BENUTZERNAME.github.io/blitzblick-training/`

Diese URL kannst du der Klasse geben (als Link in Teams/SharePoint oder als QR-Code).

## QR-Code für die Kinder (zum Scannen statt Tippen)
Im Repo liegt die Datei **`qr-code.png`** – sie codiert die URL `https://zui125.github.io/Blitzrechner/`.
- PNG herunterladen (github.com/zui125/Blitzrechner → qr-code.png → Download) oder direkt im Repo anklicken.
- Ausgedruckt an die Tafel/Tür hängen oder als Bild in Teams/SharePoint posten.
- Die Kinder scannen den Code mit dem iPhone: Kamera-App auf den Code richten **oder** Kontrollzentrum → QR-Code-Scanner. Safari öffnet die Seite automatisch.
- Auf Android: Kamera-App oder Google Lens.

Zum Selber-Erzeugen (z. B. nach Aenderung der URL): `python3 -c "import qrcode; qrcode.make('https://zui125.github.io/Blitzrechner/').save('qr-code.png')"`

## Änderungen veröffentlichen
Nach jeder Änderung an `index.html`:
```
git add index.html
git commit -m "Beschreibung der Änderung"
git push
```
GitHub Pages aktualisiert die Seite automatisch (ca. 1 Minute später).

## Hinweis Datenschutz
Es werden keine Daten an einen Server gesendet; die Seite läuft komplett im Browser der Kinder.
Das Repo ist public – der Link ist also für jeden erreichbar, der ihn kennt („unlisted").
