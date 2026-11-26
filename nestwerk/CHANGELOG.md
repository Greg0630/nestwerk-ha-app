# Änderungen

## 0.17.3
- Stundenplan-Woche: etwas höhere Felder

## 0.17.2
- Stundenplan-Fenster: „Heute“ oder „Woche“ – umschalten per Tippen oder Wischen, das Fenster behält seine Höhe

## 0.17.1
- Benachrichtigungen zu Terminen: kurzer Titel, Terminname im Text – aufgeklappt ist er jetzt vollständig lesbar
- Schul-Eintrag: gleicher Abstand zu den Terminen wie zwischen den Terminen

## 0.17.0
- Stundenplan aus Home Assistant: auf „Heute“ steht über den Terminen, wann Schule ist und was gerade läuft
- Antippen zeigt die Stunden des Tages und die ganze Woche; ohne Schule wird der nächste Schultag angezeigt

## 0.16.5
- Heute-Seite lässt sich nicht mehr ein Stück scrollen, wenn sie gar nicht voll ist

## 0.16.4
- Terminzahl oben: bei weniger Terminen rollt die neue Zahl von unten herein, bei gleich vielen oder mehr von oben

## 0.16.3
- Gestapelte Personenbilder: die erste Person liegt jetzt auch bei vielen Personen oben, mit Trennring in allen Browsern
- Screenreader lesen die Namen bei den Personenbildern vor
- Doppelt eingetragene Personen bringen die Ansicht nicht mehr zum Absturz
- Nach einem Update startet die App offline wieder richtig (keine weiße Seite mehr)
- Tipp auf eine Benachrichtigung öffnet zuverlässig die passende Seite

## 0.16.2
- Gestapelte Personenbilder bei Terminen: die erste Person liegt jetzt oben, die weiteren darunter

## 0.16.1
- Listen springen beim Eintragen/Löschen nicht mehr: „Übertrage …“ erscheint nur noch, wenn es länger dauert, und schwebt über der Navileiste

## 0.16.0
- Alle Listen außer der Einkaufsliste liegen jetzt in FamilyBoard selbst – nicht mehr in Home Assistant, nicht für Alexa/Assist sichtbar
- Bestehende, von der App angelegte Listen werden beim ersten Start mit allen Einträgen, Notizen und Anhängen übernommen und danach in Home Assistant gelöscht

## 0.15.32
- Listen nur für dich: „Mitteilungen“ im Menü ausgeblendet (niemand sonst kann sie auslösen)
- Abgehakte Einträge verschwinden zuverlässig, auch wenn die Live-Verbindung der App kurz hängt

## 0.15.31
- Kalender: der heutige Tag hat oben und unten eine Linie
- Listen: Trennlinien unter den Kategorien etwas dünner

## 0.15.30
- Benachrichtigungen: kein Ein/Aus-Knopf mehr – was abgehakt ist, ist auf diesem Gerät aktiv
- Neues Häkchen „Termine (wenn im Termin aktiviert)“: Erinnerungen lassen sich einzeln abschalten

## 0.15.29
- Admin-Passwort vergessen: neues Passwort über die App-Einstellungen in HA setzen (Feld `admin_password_reset`)
- Mengen ausgeschaltet: auch schon eingetragene Mengen werden ausgeblendet

## 0.15.28
- Neue Liste: ohne Auswahl der Listenart (startet ohne Mengen), „Speichern“ neben dem Namen, Fenster schiebt sich ganz über die Tastatur
- Listenmenü: „Einkaufsliste (Mengen)“ heißt jetzt „Mengen anzeigen“
- Erinnerungen zeigen nur noch die Uhrzeit, ohne „in 30 Min.“
- Mehrtägige Termine behalten beim Bearbeiten ihr Enddatum
- Login-Sperre pro Gerät, zusätzlich Obergrenze an Fehlversuchen
- Nach Ändern von PIN/Passwort werden Mitteilungen der anderen Geräte abgemeldet

## 0.15.27
- Hinweis „Erledigt – Rückgängig“ passt in eine Zeile

## 0.15.26
- Termin-Fenster: Speichern beim Schließen zuverlässiger
