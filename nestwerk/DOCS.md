# Nestwerk

Familien-App für gemeinsame Einkaufslisten und den Familienkalender.

## Ersteinrichtung

1. App starten und das **Protokoll** öffnen.
2. Dort steht `Einrichtungscode: XXXXXXXX`.
3. Im Heimnetz `http://<HA-IP>:8765` öffnen, Code eingeben und den ersten
   Elternteil anlegen.
4. Unter **Ich** die weiteren Familienmitglieder anlegen.

Erst nach der Einrichtung von außen erreichbar machen (z. B. Cloudflare Tunnel
auf `http://<HA-IP>:8765`).

## Daten

Alle App-Daten liegen in `/data` und sind Teil der HA-Backups.
