# Änderungen

## 0.20.2
Sicherheitsprüfung:
- Push-Abos nur noch für echte Push-Dienste (kein beliebiges Ziel im Heimnetz)
- Kinder entfernen Home-Assistant-Listen nur aus der App, nicht in HA
- Rezeptsammlungen löschen nur Eltern
- Ersteinrichtung kann nicht doppelt laufen

## 0.20.1
- Escape schließt nur das oberste Fenster (Rückfrage, Kochmodus) statt aller darunter
- Kalender: beim schnellen Blättern keine Termine aus dem falschen Monat
- Einkaufsliste: „Rückgängig“ nach dem Abhaken klappt auch bei offline eingetragenen Einträgen
- Kochmodus: kein Absturz bei doppelten Zutaten/Timern; Wecker piept auch nach mehreren Timern
- Teilen: spätes Rezept-Ergebnis schaltet nicht mehr ungefragt um; neue Liste braucht einen Namen
- Eintrag: Hinweis, wenn ohne Namen gespeichert werden soll
- Startseite: über Mitternacht offen – der gezeigte Tag bleibt derselbe

## 0.20.0
Prüfung des Codes – Fehler behoben:
- Rezept-Import: Schutz vor Abrufen im Heimnetz verschärft (IPv6-Schreibweisen, DNS-Rebinding), Größenlimit beim Lesen, ungültige Zeichen brechen nicht mehr ab, mehr Seiten werden erkannt
- Rezepte: Mengen wie „1/2 TL“ und „1 1/2 kg“ werden richtig gelesen
- Listen: geleerte Notiz bleibt leer (auch bei HA-Beschreibung); Notizen und Fotos bleiben, wenn HA kurz eine leere Liste meldet; abgelehnte Änderungen speichern nichts; entfernte Listen nehmen Vorschläge, Notizen und Anhänge mit; fehlgeschlagenes Hinzufügen hinterlässt nichts
- Offline vorgemerkte Änderungen gehen bei abgelaufener Anmeldung nicht mehr verloren
- Kalender: Suche über mehr als 400 Tage geht wieder; beim Verschieben einer Serie wandern Ausfälle mit; .ics-Import: abgesagte Serientermine, Outlook-Zeitzonen in Ausnahmen, kein doppelter Import; HA-Import: Serien mit fester Anzahl enden richtig
- Login-Bremse lässt sich im Heimnetz nicht mehr umgehen; iCal-Links nach 5 MB abgebrochen
- Benachrichtigungen: Erinnerungen auch für Termine, die kurz vorher in Google angelegt wurden; „morgen“ bei Terminen nach Mitternacht; keine doppelten Meldungen bei Änderungen von außen; vorgezogene Termine heißen „geändert“; Versandfehler bringen den Server nicht mehr zum Absturz

## 0.19.5
- Kochmodus: Schritte in ruhigerer Schrift (kleiner, halbfett, mehr Zeilenabstand) – lange Schritte passen besser

## 0.19.4
- Teilen: Fenster öffnet erst, wenn die Prüfung fertig ist, gleich in fertiger Größe (kein kurzes kleines Fenster mehr); „Link wird geprüft …“ nur, wenn es länger als 1,5 s dauert

## 0.19.3
- Teilen: erst „Link wird geprüft …“, dann direkt das passende Fenster (kein kurzes Aufblitzen des Listen-Formulars)

## 0.19.2
- Rezept: ausgewählte Zutaten kommen immer auf die Einkaufsliste (ohne Listenauswahl), Knopf „Auf Einkaufsliste“

## 0.19.1
- Teilen-Menü: bei erkanntem Rezept Umschalter „Als Rezept | Auf Liste“ mit Vorschau; der Haken speichert das Gewählte
- Rezept-Titel ohne Zusätze wie „Rezept des Tages 12.11.2015“ oder „| Chefkoch“
- Mehrzeilige Felder wachsen mit dem Text (kein Scrollbalken mehr im Notiz-Feld)

## 0.19.0
- Neuer Listentyp „Rezepte“: Rezeptsammlung mit Zutaten (Portionen umrechnen, fehlende Zutaten auf die Einkaufsliste) und Zubereitung
- Kochmodus: ein Schritt je Seite, Zutaten des Schritts, Timer; Bildschirm bleibt an
- Rezepte von Hand anlegen oder aus einem Link übernehmen (z. B. Rezeptwelt, Cookidoo – dort ohne Zubereitung, Thermomix-Blogs); auch über das Teilen-Menü

## 0.18.2
- Seite „Ich“: ohne Überschrift, obere Linie und Hinweistext; Familienbilder etwas größer und mittig unter dem Profilbild, „Bearbeiten“ bündig

## 0.18.1
- Links in Notizen sind klickbar („Link: domain.de ↗“) – in Listen direkt, bei Terminen unter dem Notiz-Feld
- Teilen-Menü: eine dabei neu angelegte Liste ist zunächst nur für dich sichtbar

## 0.18.0
- Teilen (Android): FamilyBoard erscheint im Teilen-Menü; Geteiltes landet auf einer bestehenden oder neuen Liste (Link als Notiz, mehrere Zeilen auf Wunsch als einzelne Einträge). Dafür die App einmal neu auf den Startbildschirm legen.

## 0.17.9
- Termin-Formular: Speichern per Haken oben rechts statt ✕; „Speichern“ und „Abbrechen“ unten entfallen (Abbrechen per Wischen)
- „Weitere Angaben“ in Akzentfarbe, ohne Trennlinie
- Alle einzeiligen Felder im Formular gleich hoch (auch Erinnerung bei ganztägig)
- Fenster: Titelzeile bleibt beim Scrollen stehen, mit dünner Linie darunter

## 0.17.8
- Dünnere Rahmen um Eingabefelder und umrandete Knöpfe

## 0.17.7
- Einzeln geänderter Serientermin zeigt beim erneuten Bearbeiten seine eigenen Angaben statt der der Serie
- Anmeldeseite: „Board“ in der Überschrift grau
- Kalender-Tagesfenster: Plus oben rechts statt ✕ (wie auf der Startseite), keine Linie unter dem letzten Termin

## 0.17.6
- Serientermine: beim Speichern und Löschen wählen, ob nur dieser Termin oder alle Termine der Serie gemeint sind
- Beim Bearbeiten einer Serie steht das Datum des angetippten Termins im Formular

## 0.17.5
- Startseite: unter dem Schul-Eintrag wieder die durchgehende Linie statt der Überschrift „Termine“

## 0.17.4
- Termin-Formular: Ort, Notiz und Wiederholen unter „Weitere Angaben“ (klappt weich auf; mit Inhalt automatisch offen)
- Termin-Fenster nur so hoch wie nötig
- Startseite: kleine Überschrift „Termine“ zwischen Schul-Eintrag und Terminen

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
