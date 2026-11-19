# FamilyBoard

Familien-App für gemeinsame Einkaufslisten und den Familienkalender.

## Ersteinrichtung

1. App starten und das **Protokoll** öffnen.
2. Dort steht `Einrichtungscode: XXXXXXXX`.
3. Im Heimnetz `http://<HA-IP>:8765` öffnen, Code eingeben und den ersten
   Elternteil anlegen.
4. Unter **Ich** die weiteren Familienmitglieder anlegen.

Erst nach der Einrichtung von außen erreichbar machen (z. B. Cloudflare Tunnel
auf `http://<HA-IP>:8765`).

## Google Kalender

1. In der Google Cloud Console einen OAuth-Client (Typ „Webanwendung“) anlegen,
   Weiterleitungs-URI: `https://<deine-domain>/api/google/callback`.
   Den Zustimmungsbildschirm auf **In Produktion** stellen, sonst läuft der
   Zugang nach 7 Tagen ab.
2. Hier unter **Konfiguration** `google_client_id` und `google_client_secret`
   eintragen, speichern und die App neu starten.
3. In der App unter **Ich → Kalender** „Mit Google verbinden“ (über die Domain,
   nicht über die IP) und den Familienkalender wählen.
4. Darunter festlegen, welche HA-Kalender erscheinen (z. B. Ferien als Band).

## Daten

Alle App-Daten liegen in `/data` und sind Teil der HA-Backups.
