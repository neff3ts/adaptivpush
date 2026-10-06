# Datenschutzerklärung — Adaptiv.Push

*Stand: 6. Oktober 2026*

## Kurzfassung

Deine Trainingsdaten bleiben auf deinem Gerät. Es gibt keine Werbung, kein
Tracking und keinen Verkauf von Daten. Weitergegeben wird nur an
Dienstleister, die im Auftrag des Entwicklers arbeiten, und nur, wenn du es
einschaltest.

Ab Werk verlässt nichts das Gerät. Drei Dinge kannst du selbst einschalten:
den Abgleich mit deiner **privaten** iCloud, eine **Nutzungsstatistik** und
eine **Datenspende** deiner Sätze. Statistik und Spende kommen ohne Namen
und ohne Konto aus.

Alles davon ist **freiwillig**. Die App funktioniert ohne jede dieser
Funktionen vollständig, und du musst kein Konto anlegen.

## Was auf dem Gerät bleibt

- **Trainingsverlauf**: Einheiten, Sätze, Wiederholungen, Tiefenquote,
  Volumenlast, Zeitstempel.
- **Messwerte**: Abstände der Tiefenkamera und Bewegungsdaten während eines
  Satzes. Die Messwerte der Sätze legt die App vorübergehend in ihrem
  Zwischenspeicher ab; iOS räumt ihn von selbst auf.
- **Profil**: Vorname, Kapazität, Ziel, Körpergewicht, Trainingstage,
  Übungsvariante.

Diese Daten werden lokal gespeichert.

**Der iCloud-Abgleich ist ab Werk ausgeschaltet.** Schaltest du ihn ein — im
Onboarding oder später unter *Profil* —, gleicht Apple die Daten zusätzlich
mit deiner **privaten** iCloud ab. Abgeglichen werden zwei Dinge:

- **Deine Einheiten** über die private CloudKit-Datenbank.
- **Dein Profil** — Vorname, Kapazität, Ziel, Körpergewicht, Trainingstage,
  Übungsvariante und deine Messwerte für Ober- und Unterpunkt — über
  Apples Schlüssel-Wert-Speicher. Damit beginnt das Onboarding auf einem
  neuen Gerät nicht von vorn.

Der Entwickler hat auf beides keinen Zugriff; beide Ablagen sind
ausschließlich deinem Apple-Konto zugeordnet. Ausschalten beendet den
Abgleich; was bereits in deiner iCloud liegt, verwaltest du dort.

## Kamera

Beim Training liegt das iPhone unter dir auf dem Boden. Die Frontkamera
zählt deine Liegestütze auf zwei Wegen:

- Die **TrueDepth-Kamera** misst den Abstand zu deiner Brust.
- Aus dem Bild der Frontkamera wird nur die **mittlere Helligkeit**
  berechnet. Kommt die Brust herunter, wird das Bild dunkel.

Ausgewertet wird **ausschließlich auf dem Gerät**, und zwar nur diese
beiden Werte; das Bild selbst wird sofort verworfen. Die App erkennt
weder Gesichter noch Personen oder deine Körperhaltung.

**Es wird kein Video und kein Einzelbild gespeichert, und nichts davon
verlässt das Gerät.**

## Apple Health

**Ab Werk ausgeschaltet.** Erst wenn du es einschaltest, fragt die App zwei
getrennte Berechtigungen an:

- **Lesen**: dein Körpergewicht, um die Last je Wiederholung zu berechnen.
- **Schreiben**: deine Einheiten als Workout.

Gesundheitsdaten werden **nicht** an den Entwickler oder an Dritte
übertragen.

## Nutzungsstatistik (freiwillig)

**Ab Werk ausgeschaltet.** Schaltest du unter *Profil* in der Karte *Was
dein Gerät verlassen darf* die *Nutzungsstatistik* ein, meldet die App
zwei Ereignisse:

| Ereignis | Mitgesendet |
|---|---|
| Einstieg abgeschlossen | — |
| Einheit beendet | Zahl der Wiederholungen und Sätze, Messart (welcher Sensor gezählt hat) |

Dazu kommen technische Angaben, die der Statistikdienst selbst erhebt:
App-Version, iOS-Version, Gerätemodell, Sprache und Region sowie eine
**pseudonymisierte Gerätekennung**. Der Statistikdienst macht die Kennung
auf dem Gerät mit einer Einwegfunktion (Hash) unkenntlich, bevor sie
gesendet wird, und hasht sie auf dem Server ein weiteres Mal. Name,
Apple-ID oder Telefonnummer stecken nicht darin. Sie dient nur dazu,
Ereignisse desselben Geräts zusammenzuzählen.

**Wie die Daten einzuordnen sind:** Beim Senden behandeln wir sie als
**pseudonym** und fragen deshalb nach deiner Einwilligung. Bei
TelemetryDeck kommen sie so an, dass weder TelemetryDeck noch der
Entwickler sie einer Person zuordnen kann: Die ursprüngliche Kennung
bleibt auf deinem Gerät, und IP-Adressen werden nach Angabe von
TelemetryDeck weder in der Datenbank noch in Protokolldateien gespeichert.
Für beide sind die gespeicherten Daten damit **anonym**.

**Nicht gesendet werden**: Name, Ziel, Körpergewicht, Datum und Uhrzeit
einzelner Einheiten, Messwerte, Kamerabilder, Gesundheitsdaten.

Die Daten werden nicht mit deiner Person verknüpft, nicht zum Tracking und
nicht für Werbung verwendet. Sie beantworten Fragen über die App — etwa,
wie viele den Einstieg abbrechen —, nicht über dich.

**Ausschalten** beendet das Senden sofort.

**Speicherdauer**: TelemetryDeck legt für die gespeicherten Ereignisse
keine feste Löschfrist fest und rechnet nach eigener Angabe mit einer
Löschung nach sieben bis zehn Jahren. Weil sie niemandem zugeordnet werden
können, lassen sie sich auch nicht gezielt für dich löschen (siehe *Daten
löschen*).

**Rechtsgrundlage** ist deine Einwilligung (Art. 6 Abs. 1 lit. a DSGVO,
§ 25 Abs. 1 TDDDG). Du kannst sie jederzeit mit dem Schalter widerrufen.
Der Widerruf gilt für die Zukunft; was bis dahin gesendet wurde, bleibt
rechtmäßig verarbeitet.

**Auftragsverarbeiter**: TelemetryDeck GmbH, Deutschland. Die Daten werden
in der Europäischen Union verarbeitet.

## Datenspende (freiwillig)

**Ab Werk ausgeschaltet.** Schaltest du im Onboarding oder unter *Profil* in
der Karte *Was dein Gerät verlassen darf* den Schalter *Daten spenden, um
die App zu verbessern* ein, sendet die App deine Sätze ohne Namen und
ohne Konto an einen Server. Sie dienen ausschließlich dazu, die
Berechnungen der App zu prüfen und zu verbessern — etwa wie gut die App einschätzt, wie viele
Wiederholungen noch gegangen wären.

Gesendet wird je Satz:

| Was | Warum |
|---|---|
| Wiederholungen (ganz, halb, verworfen) und Vorgabe | Wie gut Planung und Zählung treffen |
| Dauer jeder Wiederholung, Satzdauer, Pause davor | Tempoverlust als Maß für die Ermüdung |
| Geschätzte und von dir angegebene Reserve | Die Schätzung an echten Angaben prüfen |
| Übungsvariante, Messart, iPhone-Modell, App-Version | Die Messung unterscheidet sich je Gerät |
| Abstand zur vorigen Einheit in Tagen | Erholung zwischen den Einheiten |
| Ob es ein offenes Training war, ob die Tiefe messbar war | Einordnung |

Dazu eine **zufällige Spender-ID**, die nur dein Gerät kennt. Sie hängt an
keinem Konto und enthält nichts, was dich benennt. Weil sie die Sätze eines
Geräts zusammenhält, sind die Daten rechtlich **pseudonym**, nicht anonym:
Der Entwickler weiß nicht, wer hinter einer ID steht, dein Gerät kann sie
aber zuordnen. Das macht das Löschen möglich.

**Nicht gesendet werden**: Datum und Uhrzeit, Körpergewicht, Ziel, Vorname,
E-Mail-Adresse, Sensor-Rohdaten, Kamerabilder, Gesundheitsdaten aus Apple
Health.

Beim Einschalten werden auch deine bisherigen Einheiten gespendet. Eine
Einheit geht frühestens eine Stunde nach ihrem Ende hinaus, damit deine
Angabe zum letzten Satz dabei ist.

**Ausschalten** beendet das Senden. **Gespendete Daten löschen** (in
derselben Karte) löscht alles, was dein Gerät gespendet hat, vom Server und
vergisst die Spender-ID.

**Speicherdauer**: Gespendete Sätze werden gelöscht, sobald du *Gespendete
Daten löschen* tippst, spätestens aber **drei Jahre** nach ihrem Eingang
auf dem Server. Ältere Sätze löscht der Server jeden Tag von selbst.

**Rechtsgrundlage** ist deine ausdrückliche Einwilligung (Art. 6 Abs. 1
lit. a und, soweit Trainingsdaten als Gesundheitsdaten gelten, Art. 9
Abs. 2 lit. a DSGVO), für das Speichern der Spender-ID auf deinem Gerät
zusätzlich § 25 Abs. 1 TDDDG. Du kannst sie jederzeit mit dem Schalter
widerrufen. Der Widerruf gilt für die Zukunft; was bereits gespendet ist,
löschst du mit *Gespendete Daten löschen*.

**Auftragsverarbeiter**: Supabase Pte. Ltd., Singapur. Die Daten liegen in
einem Rechenzentrum in Frankfurt am Main. Weil Supabase seinen Sitz
außerhalb der EU hat und Unterauftragnehmer auch in den USA einsetzt, ist
ein Zugriff von dort, etwa für Betrieb und Support, nicht ausgeschlossen.
Abgesichert ist das durch die Standardvertragsklauseln der
EU-Kommission (Art. 46 Abs. 2 lit. c DSGVO), die Teil des
Auftragsverarbeitungsvertrags von Supabase sind. Lesen kann die Daten nur
der Entwickler für die Auswertung, kein anderer Nutzer.

## Daten löschen

Dein Trainingsverlauf liegt auf deinem Gerät und — wenn du den Abgleich
eingeschaltet hast — in deiner privaten iCloud. Unter *Profil* →
*Alle Trainingsdaten löschen* entfernst du ihn auf einmal, vom Gerät und
bei eingeschaltetem Abgleich auch aus deiner iCloud; im selben Schritt
kannst du gespendete Daten mitlöschen. Löschst du nur die App, ist der
Verlauf vom Gerät entfernt; was in iCloud liegt, löschst du dann in den
iCloud-Einstellungen deines iPhones. Vorher kannst du den vollständigen
Verlauf unter *Profil* in der Karte *Was dein Gerät verlassen darf* als
CSV oder JSON exportieren.

Die Nutzungsstatistik können weder der Entwickler noch TelemetryDeck einer
Person zuordnen, sie lässt sich deshalb auch nicht gezielt für dich löschen
(Art. 11 DSGVO). Ausschalten beendet das Senden.

Gespendete Sätze löschst du in der App mit *Gespendete Daten löschen*;
nach drei Jahren löscht der Server sie ohnehin. Ohne die Spender-ID auf deinem Gerät — etwa nachdem du die App gelöscht
hast — lassen sie sich dir nicht mehr zuordnen.

## Kein Tracking

Die App enthält keine Werbe-Kennungen, keine Absturzberichtsdienste und
keine Fremdbibliotheken, die Daten zu Werbe- oder Trackingzwecken sammeln.
Es findet kein App-übergreifendes Tracking statt.

**Absturzberichte von Apple:** Hast du in den iOS-Einstellungen unter
*Datenschutz & Sicherheit → Analyse & Verbesserungen* zugestimmt, Daten mit
App-Entwicklern zu teilen, stellt Apple dem Entwickler Absturzberichte und
zusammengefasste Nutzungszahlen bereit. Das regelt Apple nach seiner
eigenen Datenschutzrichtlinie; die App selbst sendet dafür nichts.

## Keine automatisierten Entscheidungen

Die App passt deinen Trainingsplan an deine Leistung an. Das geschieht auf
deinem Gerät und hat keine rechtliche oder ähnlich erhebliche Wirkung für
dich. Eine automatisierte Entscheidung im Sinne von Art. 22 DSGVO findet
nicht statt.

## Kontakt per E-Mail

Schreibst du dem Entwickler, verarbeitet er deine E-Mail-Adresse und den
Inhalt deiner Nachricht, um deine Anfrage zu beantworten. Rechtsgrundlage
ist Art. 6 Abs. 1 lit. b DSGVO, wenn es um die Nutzung der App geht, sonst
sein berechtigtes Interesse, Anfragen zu beantworten (Art. 6 Abs. 1 lit. f
DSGVO). Empfänger ist nur der E-Mail-Anbieter des Entwicklers als
Auftragsverarbeiter. Die Nachricht wird gelöscht, sobald die Anfrage
erledigt ist, es sei denn, eine gesetzliche Aufbewahrungspflicht besteht.

## Diese Webseite

Diese Seiten liegen bei GitHub Pages (GitHub, Inc., USA). Beim Aufruf
verarbeitet GitHub technisch notwendige Daten, insbesondere deine
IP-Adresse, um die Seite auszuliefern und vor Missbrauch zu schützen.
Rechtsgrundlage ist das berechtigte Interesse an einer sicheren
Bereitstellung (Art. 6 Abs. 1 lit. f DSGVO). GitHub ist nach dem
EU-US Data Privacy Framework zertifiziert. Die Webseite setzt keine Cookies
und keine Statistik ein. Mehr dazu im
[Datenschutzhinweis von GitHub](https://docs.github.com/de/site-policy/privacy-policies/github-general-privacy-statement).

## Kinder

Die App richtet sich nicht an Kinder. Die Nutzungsstatistik und die
Datenspende setzen deine Einwilligung voraus; dafür musst du mindestens
16 Jahre alt sein (Art. 8 DSGVO).

## Deine Rechte

Soweit der Entwickler Daten über dich verarbeitet, hast du das Recht auf

- **Auskunft** (Art. 15 DSGVO),
- **Berichtigung** (Art. 16 DSGVO),
- **Löschung** (Art. 17 DSGVO),
- **Einschränkung der Verarbeitung** (Art. 18 DSGVO),
- **Datenübertragbarkeit** (Art. 20 DSGVO),
- **Widerspruch** gegen Verarbeitungen, die auf einem berechtigten
  Interesse beruhen (Art. 21 DSGVO), etwa bei dieser Webseite oder bei
  E-Mails,
- **Widerruf** einer Einwilligung mit Wirkung für die Zukunft (Art. 7
  Abs. 3 DSGVO), in der App mit dem jeweiligen Schalter.

Vieles davon erledigst du selbst: Export des Verlaufs in der App, Löschen
auf dem Gerät, *Gespendete Daten löschen*. Für alles Weitere:
[adaptiv.push@steffenbastian.de](mailto:adaptiv.push@steffenbastian.de).

Du hast außerdem das Recht, dich bei einer Datenschutz-Aufsichtsbehörde zu
beschweren (Art. 77 DSGVO), etwa bei der Behörde deines Bundeslands.
Zuständig für den Entwickler ist der [Landesbeauftragte für den
Datenschutz und die Informationsfreiheit
Baden-Württemberg](https://www.baden-wuerttemberg.datenschutz.de).

## Verantwortlich

Steffen Bastian  
Bortkelter 7  
69226 Nussloch  
E-Mail: [adaptiv.push@steffenbastian.de](mailto:adaptiv.push@steffenbastian.de)

Weitere Angaben im [Impressum](impressum).

## Änderungen

Wesentliche Änderungen werden in der App angekündigt. Die jeweils gültige
Fassung steht unter dieser Adresse.
