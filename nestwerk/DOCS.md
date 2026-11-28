# FamilyBoard

Familien-App für gemeinsame Einkaufslisten und den Familienkalender.

## Ersteinrichtung

1. App starten und das **Protokoll** öffnen.
2. Dort steht `Einrichtungscode: XXXXXXXX`.
3. `http://<HA-IP>:8765` öffnen, Code eingeben und den ersten Elternteil anlegen.
4. Unter **Ich** die weiteren Familienmitglieder anlegen.

## Google Kalender

1. In der Google Cloud Console einen OAuth-Client (Typ „Webanwendung“) anlegen,
   Weiterleitungs-URI: `https://<deine-domain>/api/google/callback`.
   Den Zustimmungsbildschirm auf **In Produktion** stellen, sonst läuft der
   Zugang nach 7 Tagen ab.
2. Hier unter **Konfiguration** `google_client_id` und `google_client_secret`
   eintragen, speichern und die App neu starten.
3. In der App unter **Ich → Kalender** auf „Mit Google verbinden“ tippen
   (über die Domain, nicht über die IP) und den Familienkalender wählen.
4. Darunter festlegen, welche HA-Kalender angezeigt werden (z. B. Ferien als
   Band, Handball für ein Kind).

## Admin-Passwort vergessen

1. In HA: Einstellungen → Apps → FamilyBoard → Konfiguration.
2. Bei `admin_password_reset` ein neues Passwort eintragen (mind. 8 Zeichen), speichern, App neu starten.
3. Mit dem neuen Passwort anmelden; alle bisherigen Admin-Sitzungen sind abgemeldet.
4. Das Feld wieder leeren und speichern – solange es gefüllt ist, zeigt die App einen Hinweis.

## Zugriff von außen

Cloudflare Tunnel: `familie.pibuddy.de` → `http://192.168.178.99:8765`.

## Daten

Alle App-Daten liegen in `/data` und sind Teil der HA-Backups.
