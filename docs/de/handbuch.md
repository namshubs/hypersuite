# hypersuite 2.2 – Handbuch

**Erfassen · Ordnen · Mails umziehen.** Ihre Dateien und Ihre Outlook-Mails aus
einer Windows-Umgebung – aufbereitet, geordnet und sofort wieder nutzbar.

Version 2.2.2 · November 2026 · für Windows 10 und 11 (64 Bit)

<!-- pdf:part -->
## Teil I – Was hypersuite für Sie tut

Jeder Windows-Rechner sammelt über die Jahre ein eigenes kleines Universum an:
Fotos vom Handy und von drei alten Kameras, Musik von CDs und Downloads,
Rechnungen, Verträge und Steuerunterlagen, Filme, Sicherungskopien von
Sicherungskopien – verteilt auf die interne Platte, zwei USB-Festplatten, einen
Stapel Sticks und einen Cloud-Ordner. Dazu ein Outlook-Postfach mit zwanzig
Jahren Korrespondenz in einer einzigen, schwer zugänglichen PST-Datei.

**hypersuite bringt das alles in Ordnung – und auf ein Medium Ihrer Wahl.**
Das Programm erfasst jede Datei auf allen Laufwerken, findet Doppeltes, sortiert
den gesamten Bestand in eine klare, für Menschen lesbare Ordnerstruktur und
spielt sie zum Beispiel auf eine Backup-Festplatte. Das Ergebnis sind ganz
normale Windows-Ordner und -Dateien: Sie öffnen sie im Explorer, mit der
Fotoanzeige, mit Word oder dem Mediaplayer – **sofort, ohne Spezialsoftware,
ohne Import, ohne proprietäres Archivformat.**

Und Ihre Mails? Die bringt hypersuite aus Outlook nach **Thunderbird – mit der
kompletten Ordnerstruktur 1:1.** Posteingang, Gesendete Elemente und jeder
selbst angelegte Unterordner erscheinen in Thunderbird genau so, wie Sie sie in
Outlook gepflegt haben, samt allen Anhängen.

Alles in **einer einzigen Programmdatei**: keine Installation, keine
Administratorrechte, keine Cloud, kein Konto. hypersuite arbeitet vollständig
auf Ihrem Rechner und baut keine einzige Netzwerkverbindung auf.

### Wofür sich hypersuite besonders eignet

- **Umzug auf einen neuen PC** – alles Wichtige vom alten Rechner geordnet
  sichern und auf dem neuen sofort weiterverwenden.
- **Backup mit System** – statt Kopien ungeordneter Kopien eine saubere,
  dublettenfreie Bibliothek auf der Sicherungsplatte.
- **Aufräumen nach Jahren** – sehen, was wirklich doppelt ist, auf welchen
  Laufwerken, in welchen Ordnern.
- **Abschied von Outlook** – ein Postfach oder ein ganzes Archiv aus PST-Dateien
  nach Thunderbird übernehmen, ohne dass ein Ordner verloren geht.
- **Nachlass und Firmenauflösung** – die Daten eines Rechners vollständig,
  nachvollziehbar und geordnet übergeben.
- **Rettung von einer altersschwachen Platte** – eine Festplatte, die nach
  einigen Minuten heiß wird und sich abmeldet, Stück für Stück auslesen, bis
  alles Lesbare in Sicherheit ist.

<!-- pdf:module scan -->
### Scan – das Gedächtnis Ihrer Laufwerke

**Bevor man ordnet, muss man wissen, was da ist.** Scan liest jedes Laufwerk,
jeden Ordner, jede Datei und legt ein präzises Verzeichnis an: Name, Ort, Größe,
Datum – und einen digitalen Fingerabdruck des Inhalts (BLAKE3-Prüfsumme). Zwei
Dateien mit gleichem Fingerabdruck sind bitgenau identisch, egal wie sie heißen
und wo sie liegen.

**Scan vergisst nichts.** Ein USB-Stick, den Sie heute einlesen und nächsten
Monat wieder abziehen, bleibt im Verzeichnis – erkannt an seiner Seriennummer,
nicht am Laufwerksbuchstaben. So findet Scan Dubletten über alles hinweg, was Sie
je erfasst haben, auch über Datenträger, die gerade in der Schublade liegen.

**Scan ist schnell, wenn es darauf ankommt.** Beim zweiten Durchgang liest es nur
noch, was sich geändert hat. Ein unterbrochener Scan – Stromausfall, Neustart,
Fenster geschlossen – wird mit einem Klick fortgesetzt, ohne Bereits-Erfasstes
erneut zu lesen. Vorher prüft Scan, ob für sein Verzeichnis genug Platz ist, und
schlägt bei Bedarf das Laufwerk mit dem meisten freien Speicher vor.

**Scan verändert nichts.** Es liest ausschließlich. Die Berichte über doppelte
Dateien und doppelte Ordner zeigen, was sich sicher entfernen ließe – entscheiden
und löschen tun Sie selbst. Für Fotos ermittelt Scan zusätzlich das
Aufnahmedatum und – bei Bildern mit GPS-Daten – den Aufnahmeort, mit einer
eingebauten Ortsdatenbank, ohne dass je ein Standort Ihren Rechner verlässt.

**Scan rettet, was wegzufallen droht.** Eine alte Platte, die nach zehn Minuten
heiß wird, oder ein USB-Dock, das sich immer wieder abmeldet: Im
**Forensik-Modus** liest Scan nur die Dateiliste, speichert sie Ordner für
Ordner und macht nach jedem Ausfall dort weiter, wo die Platte aufgehört hat.
Sort kopiert danach die Dateien herunter – die kleinen zuerst, hängende Dateien
werden übersprungen statt abgewartet. Fällt die Platte aus, lässt hypersuite sie
abkühlen, wartet, bis sie wieder da ist, und setzt von selbst fort; nach dem
ersten Ausfall legt es die Pause schon ein, **bevor** sie wieder ausfällt.

<!-- pdf:module sort -->
### Sort – Ihre Bibliothek, sofort nutzbar

**Aus Chaos wird eine Bibliothek.** Sort nimmt alles, was Scan erfasst hat, und
baut daraus eine einzige, klar gegliederte Ordnerstruktur – auf der internen
Platte, einer externen Festplatte oder jedem anderen Ziel, das Sie wählen:

- **Fotos** nach Jahr und Monat, mit Aufnahmedatum und Ort im Dateinamen –
  RAW und JPEG, Live-Photos und Begleitdateien bleiben zusammen.
- **Musik** nach Interpret, Jahr und Album, Titel mit Tracknummer.
- **Videos** getrennt nach Filmen, Serien (Staffel, Folge) und eigenen Aufnahmen.
- **Dokumente** nach Steuer, Verwaltung, Geschäft, Familie und Ausweisen – mit
  dem Datum aus dem Dokument selbst, auf Wunsch mit Texterkennung für gescannte
  PDFs und mit einem lokalen KI-Modell, das von Ihren Beispielen lernt.
- **Alles Übrige** – Programme, Archive, Sonstiges – unverändert mit seinem
  ursprünglichen Pfad.

**Das Ergebnis sind gewöhnliche Ordner und Dateien.** Kein Container, kein
Datenbankformat, keine Abhängigkeit von hypersuite: Schließen Sie die
Backup-Platte an einen beliebigen Windows-Rechner an, und Ihre Fotos, Musik und
Dokumente sind sofort da – im Explorer, in der Fotos-App, in Word. Jede Datei
liegt genau einmal in der Bibliothek, auch wenn sie vorher fünfmal auf vier
Laufwerken verstreut war.

**Sicherheit in vier Schritten.** *Planen* – Sort legt fest, was wohin kommt,
ohne eine Datei anzufassen. *Prüfen* – Sie sehen den Plan, bevor etwas passiert.
*Ausführen* – Sort kopiert und vergleicht jede Kopie mit dem Fingerabdruck des
Originals. *Kontrollieren* – die gesamte Bibliothek wird erneut geprüft. Ihre
Originale bleiben dabei unberührt. Was sich nicht sicher einordnen lässt, wird
nicht geraten, sondern unverändert im Archiv abgelegt – verloren geht nichts.

Wer seine gewohnte Ordnerstruktur behalten möchte, schaltet auf **Spiegeln**:
Dann bringt Sort alle Laufwerke 1:1 mit ihren Original-Ordnern auf ein Ziel
zusammen – ideal als vollständige Sicherung eines alten Rechners.

<!-- pdf:module mail -->
### Outbird – Outlook nach Thunderbird, Ordner für Ordner

**Ihr Postfach zieht komplett um.** Outbird öffnet Outlook-Datendateien (PST)
direkt – Outlook muss dafür nicht einmal installiert sein – und überträgt sie in
Thunderbird, den freien Mail-Client von Mozilla.

**Die Ordnerstruktur bleibt 1:1 erhalten.** Das ist der entscheidende Vorteil:
Jeder Ordner, den Sie in Outlook über Jahre angelegt haben – Projekte, Kunden,
Jahre, Ablagen in Ablagen –, erscheint in Thunderbird in derselben Hierarchie,
mit denselben Namen, mit jeder einzelnen Nachricht. Kein Neu-Sortieren, kein
Suchen nach verschollenen Unterordnern.

**Vollständig bis ins Detail.** Absender, Empfänger, Datum und die originalen
Kopfzeilen jeder Mail, Text- und HTML-Inhalt, jeder Anhang bitgenau – auch Mails,
die als Anhang in anderen Mails stecken, samt deren eigenen Anhängen. Signierte
Nachrichten bleiben gültig signiert. Nach der Umwandlung zählt Outbird nach:
jeder Ordner, jede Nachricht wird mit der PST-Datei abgeglichen.

**Sicher für Ihr bestehendes Thunderbird.** Bevor Outbird etwas schreibt, prüft
es, dass Thunderbird geschlossen ist, und sichert Ihr komplettes
Thunderbird-Profil. Jede PST-Datei landet in einem eigenen Ordner unter *Lokale
Ordner* – mehrere Postfächer vermischen sich nicht. Alternativ exportiert Outbird
in einen eigenständigen mbox-Ordner, etwa direkt auf die Backup-Platte, ohne
Thunderbird überhaupt anzufassen.

### Gebaut für Vertrauen

- **Nur lesen, dann kopieren, dann prüfen.** Scan liest nur. Sort kopiert und
  verifiziert jede Kopie. Gelöscht wird ausschließlich auf Ihren ausdrücklichen
  Befehl – und nie eine Datei, deren Kopie nicht nachweislich stimmt.
- **Duplikate nach Inhalt.** Duplikat heißt: gleiche Größe und gleiche
  BLAKE3-Prüfsumme über den ganzen Inhalt – keine Stichproben, kein Vergleich
  nach Name oder Datum. Die Berichte empfehlen nur; gelöscht wird nichts.
- **Erst planen, dann kopieren.** Plan und Prüfen in Sort sind der Probelauf:
  Sie sehen, wohin jede Datei käme, bevor eine einzige kopiert wird.
- **Die PST bleibt unberührt.** Outbird öffnet die PST-Datei nur zum Lesen,
  sichert das ganze Thunderbird-Profil, bevor es etwas hineinschreibt, und
  schreibt nur, wenn die Umwandlung geprüft ist und Thunderbird geschlossen ist.
- **Offline.** Keine Telemetrie, keine Updates im Hintergrund, kein Konto.
  Sprachmodell, Texterkennung (Deutsch, Englisch, Französisch, Italienisch,
  Spanisch, Russisch), PDF-Darstellung und Musik-Fingerabdrücke sind eingebaut.
- **Unterbrechbar.** Jeder lange Vorgang lässt sich abbrechen und später genau
  dort fortsetzen.
- **Zweisprachig.** Oberfläche auf Deutsch und Englisch, umschaltbar mit einem
  Klick.
- **Eine Datei.** `hypersuite.exe` passt auf einen USB-Stick und läuft auf jedem
  Windows 10 und 11 ohne Installation.

<!-- pdf:part -->
## Teil II – Bedienungsanleitung

### 1. Voraussetzungen

| | |
|---|---|
| Betriebssystem | Windows 10 oder Windows 11, 64 Bit |
| Rechte | Normale Benutzerrechte genügen; keine Installation |
| Platz für das Programm | ca. 230 MB für `hypersuite.exe`, ca. 260 MB beim ersten Start für die mitgelieferten Werkzeuge |
| Platz für das Verzeichnis | ca. 1 GB je 1,3 Millionen erfasste Dateien – Scan prüft das vorab |
| Platz für die Bibliothek | bis zur Größe aller zu ordnenden Daten, da Sort kopiert |
| Für Outbird | Thunderbird (beim Übernehmen ins Profil); für den mbox-Export nicht nötig |

### 2. Herunterladen, prüfen, starten

1. Laden Sie aus dem neuesten Release auf
   <https://github.com/namshubs/hypersuite/releases/latest> die Datei
   `hypersuite.exe` und die Datei `SHA256SUMS.txt` herunter.
2. **Prüfen Sie den Download** (empfohlen). Öffnen Sie PowerShell im
   Download-Ordner und geben Sie ein:

   ```powershell
   Get-FileHash .\hypersuite.exe -Algorithm SHA256
   Get-Content .\SHA256SUMS.txt
   ```

   Der Wert für `hypersuite.exe` muss in beiden Ausgaben identisch sein.
   Die Release-Notes verlinken außerdem den **VirusTotal**-Bericht zu genau
   diesem SHA-256-Wert – das Urteil von rund 70 Virenscannern über genau diese
   Datei.
3. Legen Sie `hypersuite.exe` an einen beliebigen Ort – Downloads, ein
   Werkzeugordner oder ein USB-Stick.
4. **Doppelklick.** Beim ersten Mal zeigt Windows möglicherweise *„Der Computer
   wurde durch Windows geschützt“*. Klicken Sie auf **Weitere Informationen** und
   dann auf **Trotzdem ausführen**. Die Datei ist digital signiert (Herausgeber
   *hypersuite (github.com/namshubs/hypersuite)*); weil das Zertifikat selbst ausgestellt ist, kennt Windows es
   anfangs nicht.
5. Beim ersten Start jeder Version entpackt hypersuite für einige Sekunden seine
   Werkzeuge. Unten links erscheint dann **Mitgelieferte Werkzeuge bereit**.

> **Dem Zertifikat dauerhaft vertrauen (optional).** Laden Sie zusätzlich
> `hypersuite-codesign.cer` herunter und führen Sie in einer
> Administrator-Eingabeaufforderung aus:
> `certutil -addstore Root hypersuite-codesign.cer` und
> `certutil -addstore TrustedPublisher hypersuite-codesign.cer`.
> Danach zeigt Windows *hypersuite (github.com/namshubs/hypersuite)* als bestätigten Herausgeber.

### 3. Der Launcher

![Der Launcher](../screenshots/launcher-de.png)

Der Launcher ist die Startseite. Jede der drei Karten öffnet ein Modul in einem
eigenen Fenster:

- **Scan** – zeigt, wann zuletzt gescannt wurde und wie viele Dateien erfasst sind.
- **Sort** – zeigt das Ziel der Bibliothek und den freien Platz dort.
- **Outbird** – zeigt, wie viele PST-Dateien gefunden wurden und welches
  Thunderbird-Profil verwendet wird.

Scan und Sort können gleichzeitig geöffnet sein. Ein Klick auf die Karte eines
bereits offenen Moduls holt dessen Fenster in den Vordergrund. In der Fußzeile
finden Sie **Tools** (Zustand der mitgelieferten Werkzeuge), **About** (Version,
Lizenz, Drittsoftware) und den Sprachumschalter **DE | EN**.

#### Auto und Manuell

Viele Einstellungen tragen ein Kennzeichen: **● Auto** bedeutet, dass hypersuite
den Wert selbst ermittelt – bei jedem Start neu. Sobald Sie ihn ändern, wird er
**Manuell** und bleibt so. Ein Klick auf das Kennzeichen *Manuell* kehrt zum
automatischen Wert zurück. Unter **Advanced** finden Sie in jedem Modul alle
weiteren Optionen; **… auf Standard zurücksetzen** stellt dort alles wieder auf
Auto.

### 4. Schritt für Schritt: vom alten PC auf die Backup-Platte

Dieses Kapitel beschreibt den typischen Einsatz: Alle Dateien und das
Outlook-Postfach eines Windows-Rechners geordnet auf eine externe Festplatte
bringen, sodass alles sofort weiter nutzbar ist.

1. **Backup-Platte anschließen.** Eine leere oder ausreichend große externe
   Festplatte, z. B. Laufwerk `E:`.
2. **Scan öffnen.** Wählen Sie, was erfasst werden soll: Die Benutzerordner
   (Dokumente, Bilder, Musik, Videos, Desktop) sind vorausgewählt. Für den
   ganzen Rechner öffnen Sie **Advanced → Quellen → Alle lokalen Laufwerke**.
   Weitere Datenträger (alte USB-Platten, Sticks) anschließen und mitscannen.
3. **Scan starten.** Scan zählt zunächst die Dateien, prüft den Platz und
   erfasst dann alles. Bei großen Beständen kann das Stunden dauern – Sie können
   jederzeit abbrechen und später **Fortsetzen**.
4. **Fotos anreichern.** In Scan unter **Advanced → Fotos → Fotos anreichern**.
   Damit werden Fotos nach ihrem echten Aufnahmedatum einsortiert.
5. **Optional: Dubletten ansehen.** **Advanced → Dubletten und Berichte →
   Bericht: doppelte Ordner** zeigt, was mehrfach vorhanden ist. Für die
   Bibliothek ist das nicht nötig – Sort übernimmt jede Datei ohnehin nur einmal.
6. **Sort öffnen und das Ziel wählen.** Unter **Ziel** auf **Ändern…** klicken und
   einen Ordner auf der Backup-Platte wählen, z. B. `E:\hypersuite`.
7. **Planen, Prüfen, Ausführen, Kontrollieren** – die vier Schritte oben im
   Fenster, nacheinander. Vor dem Ausführen fragt Sort noch einmal nach.
8. **Outbird öffnen** und die Outlook-Datei übernehmen (siehe Kapitel 7):
   entweder direkt in Thunderbird oder – für die Backup-Platte – unter
   **Advanced → Ziel → mbox-Ordner** als Export nach `E:\hypersuite\mboxemails\`.
9. **Fertig.** Auf der Backup-Platte liegt jetzt eine vollständige, geordnete
   Kopie. Öffnen Sie sie im Explorer – alles ist sofort benutzbar.

> **Die Originale bleiben, wo sie sind.** Erst wenn die Bibliothek kontrolliert
> und zusätzlich gesichert ist, können Sie die Originale über *Quarantäne* und
> *Endgültig löschen* aufräumen (Kapitel 6.6). Das ist optional.

### 5. Scan im Detail

![Scan](../screenshots/scan-de.png)

#### 5.1 Was scannen

Die Schaltflächen **Dokumente, Bilder, Musik, Videos, Desktop** stehen für Ihre
Windows-Benutzerordner und sind vorausgewählt; **Downloads** ist aus. Ein Klick
schaltet einen Ordner ein oder aus. **Ordner hinzufügen** nimmt beliebige weitere
Ordner auf. Ihre Auswahl wird gespeichert.

**Laufwerke** zeigt jedes lokale Laufwerk einzeln – interne Platten ebenso wie
USB-Platten und Docks (Bezeichnung, freier Platz und „Wechseldatenträger“ beim
Darüberfahren). Ein angehaktes Laufwerk wird vollständig gescannt, zusätzlich zu
den gewählten Ordnern.

**Nicht scannen** nimmt Ordner auf, die mit allem darunter ausgelassen werden
(**Ordner ausschließen…**). Vorgeschlagen und bereits eingeschaltet sind die
Ordner, in die hypersuite selbst schreibt:

| Vorschlag | Warum |
|---|---|
| Sort-Ziel | sonst würde die fertige Bibliothek als Dublette ihrer eigenen Originale erfasst |
| `hypersuite`-Ordner | Bibliotheken früherer Läufe auf jedem Laufwerk |
| Datenbank-Ordner | das Verzeichnis selbst und seine Zwischendateien |
| Rettungsordner | Kopien aus dem Forensik-Modus (Kapitel 5.5) |
| Fotobibliothek | Bibliotheksordner von *Plan anwenden* (Fotos, unter Advanced) |

Ein Klick schaltet einen Vorschlag ab; die Wahl bleibt gespeichert. Liegt ein
Ordner, den Sie scannen wollen, **innerhalb** eines Vorschlags – etwa der
Rettungsordner selbst –, gilt dieser Vorschlag nicht und ist ausgegraut.

#### 5.2 Die Datenbank

Das Verzeichnis aller Dateien ist eine Datenbankdatei. hypersuite legt sie
automatisch an: `%USERPROFILE%\HyperindexDB\<Computer>-<Benutzer>-db\index.db`.
Scan und Sort verwenden dieselbe Datenbank.

- Unter dem Pfad steht, wie viele Dateien und Laufwerke sie enthält und wann
  zuletzt gescannt wurde.
- **Vorhandene öffnen…** verwendet eine bestehende Datenbank – etwa von einem
  früheren Lauf – und übernimmt die Ordner und Optionen ihres letzten Scans.
- **Neu anlegen…** erstellt eine neue Datenbank in einem Ordner Ihrer Wahl.
- **Zuletzt benutzt…** listet die letzten fünf Datenbanken.
- Ist eine gewählte Datei keine gültige Datenbank, erscheint sie rot, und
  **Scan starten** bleibt gesperrt.
- Reicht der Platz auf dem Laufwerk der Datenbank nicht, schlägt ein Dialog das
  Laufwerk mit dem meisten freien Speicher vor (oder **Anderer Ordner…**).

#### 5.3 Scan starten und fortsetzen

**Scan starten** zählt zuerst die Dateien (**Ohne Zählen starten** überspringt
das) und zeigt dann einen Fortschrittsbalken mit Restzeit. **Details anzeigen**
öffnet das vollständige Protokoll.

Wurde ein Scan unterbrochen, erscheint beim nächsten Öffnen die Karte **Der
letzte Scan wurde abgebrochen** mit den noch offenen Laufwerken. **Fortsetzen**
macht genau dort weiter.

Wiederholte Scans sind schnell: Unveränderte Dateien werden nicht erneut gelesen.
Regelmäßig neu zu scannen ist der vorgesehene Weg, das Verzeichnis aktuell zu
halten.

#### 5.4 Advanced

| Bereich | Option | Bedeutung |
|---|---|---|
| Quellen | Alle lokalen Laufwerke | Alle Laufwerke statt der Ordnerauswahl |
| | auch Netzlaufwerke | zusätzlich verbundene Netzlaufwerke |
| | Verknüpfungen/Junctions folgen | standardmäßig aus, um Schleifen zu vermeiden |
| | Alles neu hashen | jede Datei neu prüfen – erkennt schleichende Datenfehler |
| | Nur-online-Dateien (OneDrive) | **überspringen**: nur Name, Größe, Datum erfassen, nichts herunterladen; **herunterladen und hashen**: vollständig lesen |
| | Ordner ausschließen | Ordner**namen**, die überall übersprungen werden, z. B. `node_modules, .git` (ganze Ordner: *Nicht scannen*, Kapitel 5.1) |
| | Threads | Anzahl paralleler Leseprozesse; leer = automatisch |
| Dubletten und Berichte | Berichtsordner | Standard `Dokumente\hypersuite` |
| | Dateien ignorieren unter (Bytes) | Standard 4096 Byte |
| | Bericht: doppelte Dateien | jede Gruppe identischer Dateien, mit Empfehlung, welche bleibt |
| | Bericht: doppelte Ordner | Ordner, deren Inhalt vollständig anderswo vorhanden ist |
| Fotos | Fotos anreichern | Aufnahmedatum und Ort ermitteln (offline) |
| | Foto-Bibliothek planen / anwenden / rückgängig | eigene, reine Foto-Bibliothek; für alles andere Sort verwenden |
| Musik | Beets-Vorfilter | bereitet Musik für das Programm *beets* vor |
| Einblick | Volumes, Statistik, Aktionsprotokoll | was das Verzeichnis enthält und was geplant wurde |

Die Berichte werden als Markdown-Datei und als JSON-Datei gespeichert und löschen
nichts.

#### 5.5 Forensik-Modus: Daten von einer ausfallenden Platte retten

Manche Platten funktionieren nur noch eine Weile: Sie werden heiß, der
USB-Controller im Gehäuse steigt aus, oder das Dock trennt die Verbindung. Ein
normaler Scan liest jede Datei vollständig und verliert bei jedem Ausfall seinen
Überblick. Der Forensik-Modus ist für genau diesen Fall gebaut – in zwei
Schritten: **erst die Liste, dann die Dateien.**

**Vorbereitung**

- Datenbank und Sort-Ziel müssen auf einem **anderen** Laufwerk liegen als die
  kranke Platte. hypersuite prüft das und sperrt sonst den Start.
- Die Platte möglichst kühl aufstellen (nicht auf Teppich, Lüfter in der Nähe).
- Unter **Laufwerke** nur die kranke Platte anhaken (oder unter **Ordner
  hinzufügen** nur die Ordner darauf, die Sie brauchen).

**Schritt 1 – Scan im Forensik-Modus**

![Scan im Forensik-Modus](../screenshots/scan-forensic-de.png)

Unter **Modus** auf **Forensik** stellen. Dann gibt es zwei Einstellungen:

| Einstellung | Bedeutung |
|---|---|
| Abkühlzeit (Minuten) | so lange ruht die Platte nach einem Ausfall, Standard 10 |
| USB-Gerät neu starten … | kommt die Platte nach dem Abkühlen nicht von selbst zurück, startet hypersuite ihren USB-Anschluss neu; Windows fragt dabei einmal nach Administratorrechten |

**Scan starten** beginnt ohne Vorab-Zählung. Gelesen wird nur, was Windows im
Ordnerverzeichnis ohnehin vorhält – Name, Größe, Datum. **Keine Datei wird
geöffnet**, nichts wird geprüft, nichts wiederholt. Jeder fertig gelesene Ordner
ist sofort gespeichert.

- **Ein Ordner hängt?** Nach 30 Sekunden wird er übersprungen und im Bericht
  vermerkt; der Scan läuft weiter.
- **Die Platte fällt aus?** Die Statuszeile zeigt **Platte kühlt ab bis 14:32**,
  danach **warte auf die Platte**. hypersuite erkennt die Platte an ihrer
  Seriennummer – auch wenn Windows ihr beim Wiedereinstecken einen anderen
  Buchstaben gibt. Ist sie zurück, geht es mit dem nächsten offenen Ordner
  weiter, nicht von vorn. Erscheint sie nicht, schalten Sie das Dock aus und
  wieder ein.
- **Fenster geschlossen, Rechner neu gestartet?** Beim nächsten Öffnen zeigt
  Scan die Karte **Der Forensik-Scan wurde unterbrochen**; **Fortsetzen** macht
  beim nächsten offenen Ordner weiter.

**Schritt 2 – Dateien retten (in Sort)**

![Rettung in Sort](../screenshots/sort-rescue-de.png)

Sobald die Datenbank einen Forensik-Scan enthält, zeigt Sort über den vier
Schritten die Karte **Forensik-Scan: <Platte>** mit der Zahl und Größe der
gelisteten Dateien. **Dateien retten** kopiert sie nach

```
<Ziel>\_rescue\<Bezeichnung>-<Seriennummer>\<Originalpfad>
```

– der Ordnerbaum der Platte, nichts umbenannt, nichts einsortiert. So arbeitet
die Rettung:

- **Kleine Dateien zuerst.** In jedem Zeitfenster, das die Platte durchhält,
  kommen so möglichst viele Dateien in Sicherheit; große Videos und Images zum
  Schluss.
- **Springen statt warten.** Bewegt sich eine Kopie 20 Sekunden lang nicht,
  wird sie abgebrochen und als *übersprungen* vermerkt; sofort beginnt die
  nächste Datei. Hängen mehrere Dateien hintereinander, gilt das als Ausfall der
  Platte.
- **Abkühlen und von selbst weitermachen.** Bei einem Ausfall: Abkühlzeit,
  warten auf die Platte, gegebenenfalls USB-Neustart, dann weiter mit der
  nächsten offenen Datei.
- **Pause vor dem nächsten Ausfall.** hypersuite merkt sich, wie lange die
  Platte jeweils durchgehalten hat. Ab dem ersten Ausfall legt es die
  Abkühlpause freiwillig ein, wenn 80 % der kürzesten bisherigen Laufzeit
  erreicht sind – also bevor die Platte wieder aussteigt.
- **Zweiter Versuch.** Am Ende bekommt jede übersprungene oder unlesbare Datei
  genau einen weiteren Versuch.
- **Anhalten und Fortsetzen** sind jederzeit möglich. Kopierte Dateien werden
  nie ein zweites Mal kopiert.
- **Jede Kopie** wird zuerst als Zwischendatei geschrieben, beim Schreiben mit
  einer Prüfsumme versehen, erhält das Änderungsdatum des Originals und erst
  dann ihren richtigen Namen. Auf der kranken Platte wird nichts verändert.

Die Karte zeigt laufend **kopiert · offen · übersprungen · unlesbar**, wie oft
die Platte ausgefallen ist und, während einer Pause, bis wann sie abkühlt.
**Bericht öffnen** zeigt den Rettungsbericht
(`<Ziel>\_rescue\rescue-report-<Seriennummer>.md`): Summen, jede Arbeitsphase
mit Dauer und Grund ihres Endes, und die Liste aller Dateien, die nicht
gerettet werden konnten.

**Schritt 3 – Gerettetes ordnen**

Ist die Rettung abgeschlossen, fügen Sie in Scan den Rettungsordner unter
**Ordner hinzufügen** hinzu, stellen **Modus** wieder auf **Normal** und
scannen ihn. Jetzt werden die geretteten Dateien vollständig geprüft, Dubletten
erkannt – und Sort ordnet sie wie jede andere Quelle in die Bibliothek ein.

> **Grenzen.** Der Forensik-Modus hilft bei Platten, die wegen Hitze, Kabel,
> Dock oder USB-Controller aussteigen. Klackert eine Platte, schleift sie oder
> wird sie gar nicht mehr erkannt, ist sie mechanisch beschädigt: Dann nicht
> weiter betreiben, sondern einem Datenrettungsdienst übergeben. Dateien in
> Ordnern, deren Liste nicht lesbar war, kennt hypersuite nicht und kann sie
> nicht retten.

### 6. Sort im Detail

![Sort](../screenshots/sort-de.png)

#### 6.1 Ziel und Klassen

**Ziel** ist der Ordner der Bibliothek. Automatisch wählt Sort einen Ordner
`hypersuite` auf dem lokalen Laufwerk mit dem meisten freien Platz. Für eine
Backup-Platte wählen Sie mit **Ändern…** einen Ordner darauf. Liegt das Ziel auf
einem Laufwerk, das Sie auch gescannt haben, weist Sort darauf hin – das
funktioniert, ein separates Laufwerk ist aber sicherer.

**Was ordnen:** Fotos, Musik, Dokumente, Videos und Sonstiges – alle
vorausgewählt.

#### 6.2 Die vier Schritte

| Schritt | Schaltfläche | Was passiert |
|---|---|---|
| 1 Planen | **Plan erstellen** | Sort legt für jede Datei fest, wohin sie kommt. Nichts wird kopiert. Der Plan erhält eine Nummer und einen Bericht im Ordner `.hyperfiler\plans` des Ziels. |
| 2 Prüfen | **Plan prüfen** | Übersicht: wie viele Dateien wohin gehen und warum Dateien im Archiv oder in der Dokumenten-Inbox landen. Bericht als Markdown oder JSON öffnen. |
| 3 Ausführen | **Ausführen…** | Nach Rückfrage: Kopieren, jede Kopie gegen den Fingerabdruck prüfen, als erledigt markieren. |
| 4 Kontrollieren | **Kontrollieren** | Liest jede Datei der Bibliothek erneut und vergleicht sie. Ändert nichts. |

*Ausführen* lässt sich jederzeit unterbrechen; ein erneuter Start macht weiter,
fertige Kopien werden erkannt. Hat sich eine Quelldatei seit dem Planen
geändert, schlägt sie fehl, statt falsch kopiert zu werden – planen Sie dann neu.

**Planen bei großen Beständen** (ab 2.2.1). Planen liest jedes Dokument – bei
Scans mit Texterkennung – und kann darum Stunden dauern. Während es läuft, zeigt
Sort:

![Planen läuft: Schritt, Restzeit, Tempo und Tacho](../screenshots/sort-plan-de.png)

- **Schritt x von n** (Fotos, Musik, Dokumente, Videos, Sonstiges, Plan
  speichern) mit Balken, Dateizahl und geschätzter Restzeit, dazu die Datei, die
  gerade gelesen wird. Braucht eine Datei länger als 30 Sekunden, erscheint ein
  Hinweis – Planen arbeitet dann weiter, es hängt nicht.
- **Tempo:** ein Schieberegler von 1 bis zur Zahl Ihrer Prozessorkerne
  (Standard: die Hälfte). So viele Dokumente liest Planen gleichzeitig. Der
  Regler wirkt sofort, auch während Planen läuft; das Ergebnis ist immer
  dasselbe, nur die Dauer ändert sich. Daneben zeigt ein **Tacho** die
  CPU-Last des ganzen Rechners (Nadel) und den Anteil von Planen (farbiger
  Bogen), darunter z. B. „4 lesen · 0 KI · Sortieren wartet“.
- **Fortsetzen:** Was Planen gelesen hat, merkt es sich
  (`%LOCALAPPDATA%\hyperfiler\plan-cache.db`, nach Dateiinhalt). Wird Planen
  abgebrochen, stürzt der Rechner ab oder fällt der Strom aus, starten Sie
  einfach erneut **Plan erstellen**: Schon Gelesenes wird übersprungen. Auch ein
  zweiter Plan mit anderen Einstellungen geht dadurch viel schneller.
- **Zeitlimit je Dokument** (unter *Advanced*, Standard 120 Sekunden): Ein
  Dokument, das länger braucht, kommt unverändert ins Archiv und steht im
  Bericht („took too long to read“), statt das ganze Planen aufzuhalten.

#### 6.3 Aufbau der Bibliothek

```
E:\hypersuite\
├── Photo\2024\2024-07\20240714_Lugano_IMG_0412.jpg
├── Music\Queen\1975 - A Night at the Opera\11 - Bohemian Rhapsody.mp3
├── Video\
│   ├── Movies\Inception (2010)\Inception (2010) - 1080p.mkv
│   ├── Series\Dark (2017)\Season 01\Dark - S01E01 - Secrets.mkv
│   └── Home\2023\2023-12\20231224_Familie.mp4
├── Docs\
│   ├── Tax\2023\Steuererklärung - Finanzamt - 2024-05-02.pdf
│   ├── Administration\2024\Invoice\Stadtwerke - Invoice - 2024-03-01.pdf
│   ├── Business\Clients\<Kunde>\2024\…
│   ├── Family\2022\…
│   ├── Identity\Passport_Anna.pdf
│   └── Inbox\2024-03\Scan_017__a1b2c3d4.pdf
├── Archive\<Laufwerks-Seriennummer>\<Originalpfad>
└── .hyperfiler\   (Pläne, Quarantäne)
```

- **Fotos** werden nach Aufnahmedatum abgelegt (vorher *Fotos anreichern*); der
  Ort stammt aus GPS-Daten. RAW- und JPEG-Paare, XMP-Dateien und
  Live-Photo-Videos bleiben zusammen.
- **Musik** wird nach ihren Tags abgelegt; fehlen sie, übernimmt Sort sie von
  einer akustisch identischen Kopie, die sie hat.
- **Videos** werden am Dateinamen erkannt (`Titel (2019) 1080p`, `Serie S01E02`),
  dann an eingebetteten Daten und `.nfo`-Dateien. Alles andere gilt als eigene
  Aufnahme.
- **Dokumente** (PDF, Word `.docx`/`.doc`, OpenDocument `.odt`, Text) werden
  gelesen und nach festen Regeln eingeordnet. Was nicht sicher zuzuordnen ist,
  landet in `Docs\Inbox` – es wird nichts geraten.
- **Sonstiges** wird unverändert übernommen.
- **Archive** ist das Sicherheitsnetz: Dateien ohne verwertbare Angaben werden
  bitgenau mit ihrem Originalpfad unter der Seriennummer ihres Laufwerks
  abgelegt.

Gleichnamige, aber verschiedene Dateien bleiben beide erhalten (`-v1`, `-v2`
nach Datum bzw. mit der Laufwerks-Seriennummer). Identische Dateien landen genau
einmal in der Bibliothek.

#### 6.4 Advanced: Modus und Dokumente

- **Umorganisieren (Bibliotheks-Struktur)** – der Aufbau oben (Standard).
- **Spiegeln (Quellstruktur 1:1)** – keine Sortierung: Alles wird mit seiner
  originalen Ordnerstruktur nach `Archive\<Seriennummer>\…` kopiert. Ideal, um
  mehrere Laufwerke unverändert auf einer Backup-Platte zusammenzuführen.
- **entities.toml** – Ihre eigenen Firmen, Kunden und Personen, damit Dokumente
  unter deren Namen abgelegt werden:

  ```toml
  [[entity]]
  name = "Stadtwerke München"
  aliases = ["SWM"]
  role = "vendor"          # vendor (Absender), client (Kunde), holder (Inhaber)
  class = "administration" # tax, administration, business, family, identity

  [[entity]]
  name = "Anna Beispiel"
  role = "holder"          # wessen Pass, Ausweis oder Urkunde
  ```

- **OCR-Seiten** – gescannte PDFs bis zu dieser Seitenzahl per Texterkennung
  lesen (leer = aus; einige Sekunden pro Seite).
- **KI-Dokumentsortierung** – ein mitgeliefertes, mehrsprachiges Sprachmodell
  ordnet Dokumente ein, die sonst in die Inbox gingen. Es lernt aus Beispielen,
  die Sie mit `hypersuite file inbox-review` vergeben, und läuft vollständig
  offline.
- **genres.toml** – Ihre Zuordnung von Filmtiteln zu Genres:

  ```toml
  [movies]
  "The Matrix" = "Sci-Fi"
  "Der Pate" = "Drama"
  ```

#### 6.5 PST-Dateien im Index

Outlook-Dateien, die Scan auf Ihren Laufwerken gefunden hat, kann Sort in einem
Zug verarbeiten: **Im Index suchen**, dann **Ignorieren** (werden wie andere
Dateien archiviert), **Als mbox ins Ziel** (nach `<Ziel>\mboxemails\<Name>`) oder
**In ein Thunderbird-Profil**, und schließlich **Gefundene Mails verarbeiten**.

#### 6.6 Wartung: Quarantäne, endgültig löschen, suchen

Wenn die Bibliothek kontrolliert **und separat gesichert** ist, können die
Originale weichen – bewusst in zwei Schritten:

1. **Quarantäne** verschiebt die Originale aller geprüften Kopien nach
   `<Ziel>\.hyperfiler\quarantine\…`. Nichts wird gelöscht. Vor jedem
   Verschieben wird die Kopie in der Bibliothek noch einmal geprüft.
2. **Endgültig löschen** entfernt Dateien, die länger als die eingestellte Frist
   (Standard 30 Tage) in der Quarantäne liegen. Es ist der **einzige** Schritt in
   hypersuite, der etwas löscht. Er verlangt unter *Backup bestätigt* eine Notiz
   von Ihnen (z. B. „NAS-Sicherung 25.10.2026“) und löscht nie eine Datei, deren
   Kopie in der Bibliothek nicht mehr stimmt. Es gibt kein Rückgängig.

**Suchen** findet Dokumente nach ihrer Bedeutung statt nach exakten Wörtern –
„Kfz-Versicherung Verlängerung“ findet auch das Schreiben, in dem diese Wörter
nicht vorkommen, sprachübergreifend. Vor der ersten Suche einmal **Suchindex neu
aufbauen**.

#### 6.7 Rettung von einer ausfallenden Platte

Enthält die Datenbank einen Forensik-Scan, erscheint über den vier Schritten die
Karte **Forensik-Scan: <Platte>** mit **Dateien retten**, **Anhalten** und
**Rettung fortsetzen**. Ablauf und Einstellungen beschreibt Kapitel 5.5. Liegt
das Sort-Ziel auf der Platte, die gerettet wird, ist **Dateien retten**
gesperrt – wählen Sie dann unter **Ziel** ein anderes Laufwerk. Die Forensik-
Dateien selbst plant Sort nicht ein: Sie haben noch keine Prüfsumme und werden
erst über den Rettungsordner (Schritt 3 in Kapitel 5.5) Teil der Bibliothek.

### 7. Outbird im Detail

![Outbird](../screenshots/mail-de.png)

#### 7.1 Die PST-Datei

Outbird schlägt PST-Dateien vor, die es in den üblichen Outlook-Ordnern
(`Dokumente\Outlook-Dateien`, `%LOCALAPPDATA%\Microsoft\Outlook`) und unter den
gescannten Dateien findet. Mit **Durchsuchen…** wählen Sie jede andere. Nach der
Auswahl zeigt Outbird, wie viele Ordner und Nachrichten die Datei enthält.

> **Exchange, Microsoft 365, IMAP:** Diese Konten speichert Outlook nicht als
> PST, sondern als Zwischenspeicher (OST). Exportieren Sie das Postfach zuerst in
> Outlook: *Datei → Öffnen und exportieren → Importieren/Exportieren → In Datei
> exportieren → Outlook-Datendatei (.pst)*.

#### 7.2 In Thunderbird übernehmen

1. Unter **Nach** steht Ihr Thunderbird-Profil; automatisch das
   Standardprofil, mit **Ändern…** ein anderes.
2. **Thunderbird schließen.** Outbird prüft das.
3. Häkchen bei *Mir ist klar, dass das mein Thunderbird-Profil verändert*
   setzen, **In Thunderbird übernehmen** klicken und bestätigen.

Outbird sichert dann das ganze Profil (`outbird-backup-<Datum>` neben dem
Profilordner), wandelt die PST-Datei in einen Ordner `<Name>-thunderbird` neben
der PST-Datei um, prüft das Ergebnis Ordner für Ordner und Nachricht für
Nachricht und kopiert erst dann alles in die **Lokalen Ordner** des Profils.
Schlägt die Prüfung fehl, bleibt das Profil unberührt. Danach startet
Thunderbird – Ihre Outlook-Ordner erscheinen dort in derselben Struktur, in
einem Ordner mit dem Namen der PST-Datei.

#### 7.3 Als mbox-Ordner exportieren

**Advanced → Ziel → mbox-Ordner** schreibt einen eigenständigen Ordner mit
Thunderbird-kompatiblen mbox-Dateien – ohne eine Thunderbird-Installation
anzufassen. Ideal für die Backup-Platte. Standardort:
`<Sort-Ziel>\mboxemails\<Name der PST>`. Später lässt sich dieser Ordner in die
*Lokalen Ordner* eines Thunderbird-Profils kopieren.

#### 7.4 Advanced

| Option | Bedeutung |
|---|---|
| Alles in einen Wurzelordner | Standard ein; leer = Name der PST-Datei. Bei mehreren PST-Dateien eingeschaltet lassen, damit sich deren Posteingänge nicht vermischen. |
| Vorhandene Postfächer/Ordner überschreiben | Standard aus: Outbird bricht ab, statt zu überschreiben. |
| Testlauf | alles außer Schreiben |
| Thunderbird danach starten | Standard ein |
| Inhalt prüfen | Ordner und Nachrichtenzahlen lesen, nichts schreiben |

Outbird überträgt **E-Mails**. Kontakte und Kalendereinträge werden nicht in
Adressbuch oder Kalender von Thunderbird übernommen.

### 8. Kommandozeile (Kurzreferenz)

Alles, was die Fenster tun, steht auch auf der Kommandozeile zur Verfügung. In
der Eingabeaufforderung `start /wait` voranstellen, in PowerShell
`| Out-Host` anhängen.

```bat
start /wait hypersuite index scan E:\ --db D:\index.db
start /wait hypersuite index scan --resume
start /wait hypersuite index scan F:\ --exclude-dir F:\hypersuite --db D:\index.db
start /wait hypersuite index scan F:\ --forensic --cooldown 600 --usb-restart --db D:\index.db
start /wait hypersuite index rescue --target E:\Rettung --volume F: --db D:\index.db
start /wait hypersuite index rescue --target E:\Rettung --status --db D:\index.db
start /wait hypersuite file plan E:\hypersuite --db D:\index.db
start /wait hypersuite file apply <PLAN-NUMMER> E:\hypersuite --db D:\index.db
start /wait hypersuite mail export C:\mail\archiv.pst --root-name ""
start /wait hypersuite tools --verify
```

`hypersuite <befehl> --help` zeigt die vollständige Hilfe mit Beispielen. Die
ausführliche Referenz (englisch):
<https://github.com/namshubs/hypersuite/blob/main/docs/command-line.md>.

### 9. Dateien, Einstellungen, Datenschutz

| Was | Wo |
|---|---|
| Einstellungen | `%LOCALAPPDATA%\hypersuite\settings.json` |
| Mitgelieferte Werkzeuge | `%LOCALAPPDATA%\hypersuite\runtime\` (ältere Versionen werden entfernt) |
| Datenbank | `%USERPROFILE%\HyperindexDB\<Computer>-<Benutzer>-db\index.db` |
| Berichte von Scan | `Dokumente\hypersuite\` |
| Bibliothek | `<Laufwerk>:\hypersuite\` oder Ihr gewähltes Ziel |
| Quarantäne | `<Ziel>\.hyperfiler\quarantine\` |
| Rettungskopien (Forensik) | `<Ziel>\_rescue\<Bezeichnung>-<Seriennummer>\`, Bericht `<Ziel>\_rescue\rescue-report-<Seriennummer>.md` |
| Thunderbird-Sicherung | `%APPDATA%\Thunderbird\Profiles\outbird-backup-<Datum>\` |

hypersuite schreibt nichts in die Registry oder nach *Programme*. Die Datenbank
enthält Namen und Orte Ihrer Dateien, aber keine Inhalte – behandeln Sie sie wie
ein Inhaltsverzeichnis Ihrer Laufwerke. Den gelesenen Text Ihrer Dokumente merkt
sich Planen in `%LOCALAPPDATA%\hyperfiler\plan-cache.db`, damit es nach einem
Abbruch weitermachen kann; die Datei darf jederzeit gelöscht werden. Nichts davon
verlässt Ihren Rechner – hypersuite hat keine Netzwerkfunktion (Anhang A).

**Deinstallieren:** `hypersuite.exe` löschen, `%LOCALAPPDATA%\hypersuite\`
löschen und bei Bedarf Datenbank, Berichte und Bibliothek.

### 10. Hilfe bei Problemen

| Problem | Lösung |
|---|---|
| SmartScreen-Warnung | **Weitere Informationen → Trotzdem ausführen**, oder Zertifikat vertrauen (Kapitel 2) |
| „Werkzeuge fehlen – siehe Tools“ | **Tools → Neu entpacken**; ca. 260 MB frei in `%LOCALAPPDATA%` nötig |
| In der Eingabeaufforderung erscheint nichts | `start /wait hypersuite …` verwenden |
| Scan hängt an einer Datei | meist eine Cloud-Datei oder ein langsames Laufwerk; Ordner ausschließen oder *Nur-online-Dateien: überspringen*; Abbrechen und **Fortsetzen** verliert nichts |
| „Keine hyperindex-Datenbank“ | richtige Datei mit **Vorhandene öffnen…** wählen oder **Neu anlegen…** |
| Sort meldet „Erst scannen“ | zuerst Scan ausführen oder vorhandenen Index wählen |
| Viele Dokumente in `Docs\Inbox` | `entities.toml` pflegen, OCR einschalten, KI-Sortierung mit eigenen Beispielen |
| Dateien im `Archive` statt bei Fotos/Musik | vor dem Planen *Fotos anreichern*; Cloud-Dateien mit *herunterladen und hashen* scannen |
| „Thunderbird läuft“ | Thunderbird vollständig beenden (auch im Infobereich) |
| „… existiert bereits im Thunderbird-Profil“ | *Alles in einen Wurzelordner* eingeschaltet lassen oder anders benennen |
| Kein Thunderbird-Profil gefunden | Thunderbird installieren und einmal starten – oder als mbox exportieren |
| Eine Platte meldet sich nach einer Weile ab | Forensik-Modus verwenden (Kapitel 5.5) |
| Forensik: „Die Datenbank liegt auf einem Laufwerk, das gescannt wird“ | unter **Datenbank** mit **Neu anlegen…** eine Datenbank auf einem anderen Laufwerk anlegen |
| Rettung: **Dateien retten** gesperrt | das Sort-Ziel liegt auf der kranken Platte – anderes **Ziel** wählen |
| Rettung: „warte auf die Platte“ bleibt stehen | Dock bzw. USB-Gehäuse aus- und wieder einschalten; die UAC-Abfrage für den USB-Neustart bestätigen |
| Rettung: viele Dateien *übersprungen* | normal bei schwachen Sektoren; der zweite Durchgang am Ende versucht sie noch einmal, der Bericht listet den Rest |

Fehler melden und Fragen stellen: <https://github.com/namshubs/hypersuite/issues>
– gern auf Deutsch, mit der Version (`hypersuite --version`) und dem Text unter
**Details anzeigen**.

### 11. Lizenz

hypersuite steht unter der **Sustainable Use License 1.0**: kostenlos nutzbar für
private, nicht-kommerzielle und interne geschäftliche Zwecke und kostenlos
weitergebbar für nicht-kommerzielle Zwecke; hypersuite zu verkaufen oder anderen
kommerziell anzubieten ist nicht erlaubt. Keine Gewährleistung (Datei `LICENSE`,
Copyright-Hinweis in `NOTICE`). hypersuite ist **keine Open-Source-Software**; der
Quellcode ist auf Anfrage einsehbar (siehe *Quellcode und Mitarbeit*). Version
2.1.3 erschien unter der Apache License 2.0; seit 2.1.4 gilt die neue Lizenz aus
den dort genannten Gründen – eine Kopie von 2.1.3, die Sie schon haben, bleibt
unter Apache 2.0. Die mitgelieferten Komponenten von
Drittanbietern behalten ihre eigenen Lizenzen; die Liste steht im Programm unter
**About**, der Quellcode der GPL/LGPL-Komponenten liegt jedem Release als
`third-party-sources.zip` bei.

#### Nutzung auf eigene Gefahr

Die Nutzung von hypersuite erfolgt auf eigene Gefahr. Es gibt keinen geregelten
Support. Wie jede Software kann hypersuite Fehler enthalten – bewahren Sie Ihre
Originaldaten und eine unabhängige Sicherung auf, bis Sie das Ergebnis selbst
geprüft haben.

Oder, wie es der Legende nach – vermutlich vom Vater von Bill Gates, dem
Juristen – hinten auf die ersten Z-80-Emulationskarten geschrieben wurde:

> „In juristischem Sinne: Wir bestreiten, dass diese Software für einen wie auch
> immer gearteten Zweck geeignet ist.“

#### Quellcode und Mitarbeit

Entwickelt wird auf einem eigenen, unabhängigen Git-Server; veröffentlicht werden
nur die Releases und die Dokumentation. Das ist bewusst so: Der Code und seine
Kernideen sollen nicht in den Trainingsdaten großer KI-Modelle landen, und die
Richtung des Projekts bleibt in der Hand des Autors.

Rückmeldungen, Fehlerberichte und Ideen sind immer willkommen. Zugang zum
Quellcode bekommt, wer das Ziel des Projekts teilt – Menschen helfen, Outlook zu
verlassen, Windows aufzuräumen und den Umstieg auf Linux vorzubereiten – und vier
Dinge mitbringt: Mensch (keine KI als Contributor; KI als Werkzeug ist in Ordnung),
keine Verbindung zu Big Tech, Engagement für Datenschutz bzw. Nutzerrechte und
eine technische Verbesserungsagenda. Die Anfrage läuft über eine Discussion in der
Kategorie „Contributor access“ oder ein Issue mit der Vorlage *Contributor
access*; danach folgen ein interaktives Onboarding und die Unterschrift unter das
Contributor Agreement. Details: `CONTRIBUTING.md` und `CONTRIBUTOR-AGREEMENT.md`
im Ordner `.github` des Projekts.

Projekt: <https://github.com/namshubs/hypersuite>

### Anhang A: Die KI in hypersuite – lokal eingebaut, ohne Verbindung nach außen

**Kurz:** hypersuite enthält keinerlei Netzwerkfunktion. Alles, was das Programm
von Ihren Dateien liest – Namen, Prüfsummen, Text, OCR-Ergebnisse, KI-Berechnungen –,
bleibt auf Ihrem Rechner. Es gibt keine Cloud, kein Konto, keine Telemetrie, keine
Update-Prüfung und keine Absturzberichte.

#### Welche KI

hypersuite nutzt **ein einziges KI-Modell: multilingual-e5-small** (entwickelt von
Microsoft Research, veröffentlicht als `intfloat/multilingual-e5-small`, MIT-Lizenz),
in der kompakten int8-Fassung (`Xenova/multilingual-e5-small`, rund 118 MB).

Das ist **kein Chatbot und kein Sprachmodell, das Texte schreibt**. Es ist ein
sogenanntes Embedding-Modell: Es übersetzt den Anfang eines Dokuments (höchstens
512 Wortteile) in 384 Zahlen. Dokumente mit ähnlichem Inhalt bekommen ähnliche
Zahlen. Mehr kann es nicht – es erzeugt keinen Text, beantwortet keine Fragen und
lernt nicht dazu.

#### Wie sie eingebaut ist

- Die Modelldatei steckt **in `hypersuite.exe`**. Beim ersten Start wird sie
  zusammen mit den anderen Werkzeugen nach `%LOCALAPPDATA%\hypersuite\runtime\`
  entpackt und per SHA-256 geprüft.
- Gerechnet wird mit **tract**, einer Rechenbibliothek, die fest im Programm
  steckt. Es gibt keinen separaten KI-Dienst, keinen Server im Hintergrund und
  keine Grafikkarten-Treiber.
- Verwendet wird das Modell **nur** in Sort → Planen, **nur** wenn unter
  *Advanced* „KI-Dokumentsortierung“ eingeschaltet ist, **nur** für Dokumente,
  die die festen Regeln nicht sicher zuordnen, und **nur**, wenn Sie selbst
  Dokumente beschriftet haben (`labels.jsonl`). Das Modell vergleicht ein
  unsicheres Dokument dann mit Ihren beschrifteten Beispielen („nächste
  Nachbarn“). Ohne Ihre Beschriftungen rechnet Planen die KI gar nicht erst.
- Das Modell wird **nie trainiert und nie verändert** – es lernt nichts. Nach
  einem Lauf weiß es nichts über Ihre Dokumente; es ist dieselbe Datei wie
  vorher. Ihre Beschriftungen bleiben in Ihrer eigenen Datei.

Ebenfalls eingebaut und ebenfalls rein lokal: **Tesseract** (Texterkennung in
gescannten PDFs, sieben Sprachen), **PDFium** (stellt PDF-Seiten für die
Texterkennung als Bild dar) und **fpcalc** (akustischer Fingerabdruck von
Musikstücken – nur berechnet und verglichen, keine Abfrage bei einer
Online-Datenbank).

#### Warum die gelesenen Informationen das Programm nicht verlassen

- **Kein Netzwerk-Code:** hypersuite, hyperindex, hyperfiler und Outbird
  enthalten keinen Programmteil, der eine Internet- oder Netzwerkverbindung
  aufbaut – keinen HTTP-Aufruf, keine Sockets. Die Werkzeuge laufen als lokale
  Prozesse und bekommen nur lokale Dateien übergeben.
- **Keine versteckten Downloads:** Online-Platzhalter von OneDrive & Co. werden
  nie geöffnet – sonst würde Windows sie aus der Cloud nachladen.
- **Netzlaufwerke nur auf Wunsch:** Scan liest ein NAS oder Netzlaufwerk nur,
  wenn Sie es ausdrücklich einschließen. Das ist Lesen von Dateien in Ihrem
  eigenen Netz; hypersuite sendet dabei nichts nach außen.
- **Ein Hinweis zur Ehrlichkeit:** Das mitgelieferte Tesseract-Paket (Windows-Build
  von UB Mannheim) enthält die Bibliothek `libcurl`, weil Tesseract selbst Bilder
  auch von einer Webadresse laden *könnte*. hypersuite übergibt Tesseract
  ausschließlich lokale Bilddateien; diese Fähigkeit wird nie benutzt.
- **Geprüft (Version 2.2.1):** der Quellcode aller vier Teile; dazu eine Messung
  während eines Planlaufs mit Texterkennung und KI – 20 beteiligte Prozesse,
  **null** Netzwerkverbindungen.

#### Wo gelesene Inhalte gespeichert werden

| Datei | Inhalt |
|---|---|
| `index.db` (Ihre Datenbank) | Namen, Orte, Größen, Daten und Prüfsummen Ihrer Dateien, die Pläne – keine Dateiinhalte |
| `%LOCALAPPDATA%\hyperfiler\plan-cache.db` | **der gelesene Text Ihrer Dokumente** (inkl. Texterkennung) und die KI-Zahlen dazu – damit Planen fortsetzen kann |
| `%LOCALAPPDATA%\hyperfiler\fingerprints.db` | akustische Fingerabdrücke von Musikstücken |

Alle drei liegen nur auf Ihrem Rechner. `plan-cache.db` und `fingerprints.db`
dürfen Sie jederzeit löschen; Planen liest die Dokumente dann beim nächsten Mal
neu.

#### Selbst nachprüfen und erzwingen

- **Nachprüfen:** Ressourcenmonitor (`resmon`) → Reiter *Netzwerk*. Während
  hypersuite läuft, erscheinen weder `hypersuite.exe` noch `tesseract.exe` oder
  `fpcalc.exe` unter *Netzwerkaktivität* oder *TCP-Verbindungen*.
- **Erzwingen:** Wer es zusätzlich technisch absichern möchte, sperrt die
  Programme in der Windows-Firewall für ausgehende Verbindungen (PowerShell als
  Administrator, Pfad zur Exe anpassen):

```powershell
New-NetFirewallRule -DisplayName "hypersuite: kein Netz" `
    -Direction Outbound -Action Block -Program "C:\Pfad\zu\hypersuite.exe"
Get-ChildItem "$env:LOCALAPPDATA\hypersuite\runtime" -Recurse -Filter *.exe |
    ForEach-Object {
        New-NetFirewallRule -DisplayName "hypersuite: kein Netz ($($_.Name))" `
            -Direction Outbound -Action Block -Program $_.FullName
    }
```

hypersuite funktioniert mit diesen Regeln unverändert – es braucht das Netz nicht.


### Anhang B: Hilfe zu jedem Element und die passenden Befehle

Jedes Element der Fenster hat eine Erklärung: Mit der Maus darüberfahren zeigt
einen Kurztext, **Rechtsklick → „Erklärung…“** oder **F1** öffnet die
ausführliche Hilfe mit dem entsprechenden Befehl und „Befehl kopieren“. Das
Fragezeichen oben rechts erklärt das und schaltet die Kurztexte ab. Auf der
Befehlszeile gibt `hypersuite help <Thema>` denselben Text (englisch),
`hypersuite help --topics` listet alle Themen; die Schalter eines Befehls zeigt
sein `--help`. Die Texte unten sind dieselben wie im Programm.

**Wie viele Seiten je Scan per Texterkennung (OCR) gelesen werden. Leer = aus (Standard).**  
OCR liest Text aus Bildern und eingescannten PDFs, damit Dokumente nach Inhalt (Datum, Absender) einsortiert werden können. Das kostet je Seite etwa eine bis mehrere Sekunden und verlängert das Planen bei vielen Scans deutlich. Leer lässt OCR aus: dann zählt nur Text, der schon in der Datei steckt. 1 bis 3 reicht meist für Briefkopf und Datum. Schon gelesene Seiten kommen beim nächsten Planen aus dem Zwischenspeicher. Alles läuft auf deinem Rechner, nichts wird gesendet.

Befehl: `hypersuite file plan <Ziel> --ocr-pages N`  
Alle Schalter: `hypersuite file plan --help`

**Reorganisieren sortiert in die Bibliotheksstruktur, Spiegeln kopiert die Quellstruktur 1:1 ins Archiv, ohne Inhalte zu lesen.**  
Reorganisieren (Standard) ordnet jede Datei nach Art, Datum und Inhalt in die Bibliothek ein. Spiegeln überspringt jede Einordnung: Alles landet unter Archive/&lt;Laufwerks-Seriennummer>/&lt;ursprünglicher Pfad>, die Quellstruktur bleibt erhalten. Dabei werden keine Dokumente gelesen, kein OCR und keine KI verwendet, Spiegeln ist deshalb viel schneller. In beiden Fällen ist es zunächst nur ein Plan: erst „Ausführen“ kopiert.

Befehl: `hypersuite file plan <Ziel> --db <DB> --mirror`  
Alle Schalter: `hypersuite file plan --help`

**Deine bekannten Absender, Kunden und Dokumentinhaber (TOML). Hilft, Dokumente richtig zuzuordnen. Nur für Dokumente.**  
Die Datei nennt Lieferanten, Kunden und Personen, damit Dokumente nach ihnen eingeordnet werden können. Ohne die Datei ordnet Planen nur nach den eingebauten Regeln. Nur die Klasse Dokumente nutzt sie.

Befehl: `hypersuite file plan <Ziel> --db <DB> --entities entities.toml`  
Alle Schalter: `hypersuite file plan --help`

**Tabelle Filmtitel → Genre (TOML). Ein Film ohne Eintrag bekommt keinen Genre-Ordner, es wird nie geraten. Nur für Videos.**  
Mit dieser Tabelle legt Planen Filme in Genre-Unterordner. Fehlt ein Film in der Tabelle, bekommt er keinen Genre-Ordner. Es wird nie ein Genre geraten. Nur die Klasse Videos nutzt die Tabelle.

Befehl: `hypersuite file plan <Ziel> --db <DB> --genres genres.toml`  
Alle Schalter: `hypersuite file plan --help`

**Das mitgelieferte KI-Modell rettet Dokumente, die die Regeln sonst in den Eingang schicken würden. Braucht labels.jsonl, läuft lokal.**  
Das mitgelieferte Embedding-Modell vergleicht den Text eines Dokuments mit deinen gelabelten Beispielen aus labels.jsonl und ordnet es danach ein, wenn die Regeln allein es in den Eingang (Inbox) schicken würden. Es wird nichts trainiert und nichts gesendet: Das Modell läuft auf deinem Prozessor und lernt nichts dazu. Ohne labels.jsonl gibt es keine Beispiele, Planen rechnet die KI dann gar nicht erst.

Befehl: `hypersuite file plan <Ziel> --db <DB> --model --labels labels.jsonl`  
Alle Schalter: `hypersuite file plan --help`

**Beispiel-Datei (JSON Lines), die „inbox-review“ geschrieben hat. Nur mit KI-Sortierung. Standard: hyperfiler-labels.jsonl im aktuellen Ordner.**  
Das sind die Beispiele, mit denen die KI vergleicht. Du erzeugst sie mit „inbox-review“, indem du Dokumente selbst einordnest. Bleibt das Feld leer, nimmt Planen die Datei hyperfiler-labels.jsonl aus dem aktuellen Ordner, falls sie dort liegt.

Befehl: `hypersuite file plan <Ziel> --db <DB> --model --labels labels.jsonl`  
Alle Schalter: `hypersuite file plan --help`

**Nach so vielen Sekunden wird ein Dokument aufgegeben und unverändert ins Archiv gelegt. 0 = kein Limit, Standard 120.**  
Manche Dateien hängen im Parser oder brauchen beim OCR sehr lange. Nach dem Limit gibt Planen das Dokument auf: Es kommt unverändert ins Archiv und steht im Bericht mit dem Vermerk, dass es zu lange gedauert hat. Das Zeitlimit wird im Zwischenspeicher vermerkt. Die anderen Dokumente sind davon nicht betroffen.

Befehl: `hypersuite file plan <Ziel> --db <DB> --file-timeout 120`  
Alle Schalter: `hypersuite file plan --help`

**Nummer eines früheren Plans (hyperfiler-plan-…), um ihn zu prüfen oder auszuführen, ohne neu zu planen.**  
Jedes Planen bekommt eine Nummer und schreibt einen Bericht und geplante Aktionen in die Datenbank. Mit der Nummer eines früheren Plans arbeitest du an ihm weiter, ohne neu zu planen. Die Nummer steht im Bericht unter &lt;Ziel>\.hyperfiler\plans\ und in der Zeile unter dem Knopf, wenn ein Plan fertig ist.

Alle Schalter: `hypersuite file --help`

**PST-Dateien (Outlook-Postfächer) im Index werden nicht sortiert, sondern als Mail übernommen: ignorieren, als mbox oder in ein Thunderbird-Profil.**  
Ignorieren lässt die PST-Dateien, wie sie sind. Als mbox schreibt hypersuite die Mails in das Ziel. In ein Thunderbird-Profil geht den geführten Weg: Thunderbird muss geschlossen sein, das Profil wird gesichert, die Mails werden umgewandelt, geprüft und erst dann in die lokalen Ordner kopiert. Dafür bestätigst du vorher den Hinweis.

Alle Schalter: `hypersuite mail --help`

**Verschiebt die Quellen bestätigter Kopien nach .hyperfiler/quarantine. Löscht nichts; die Kopie wird vorher erneut geprüft.**  
Nur Quellen, deren Kopie geprüft („verified“) ist, werden verschoben, mit ihrem ursprünglichen relativen Pfad unter &lt;Ziel>\.hyperfiler\quarantine\&lt;Seriennummer>\. Vor jedem Verschieben wird die Kopie noch einmal per Prüfsumme kontrolliert, damit auch die einzige Quelle eines Inhalts sicher ist. Mit „Nur dieser Plan“ gilt es nur für die Quellen des gewählten Plans.

Befehl: `hypersuite file quarantine <Ziel> --db <DB> [--plan <Plan-Nummer>]`  
Alle Schalter: `hypersuite file quarantine --help`

**ENDGÜLTIG löschen: entfernt Quarantäne-Kopien nach der Wartezeit. Nicht rückgängig zu machen, braucht deine Backup-Bestätigung.**  
Das ist der einzige Schritt, der sich nicht rückgängig machen lässt. Gelöscht werden nur Quarantäne-Kopien, die mindestens so viele Tage alt sind wie angegeben (Standard 30). Das Backup-Feld ist deine eigene Bestätigung, dass es ein zweites, unabhängiges Backup gibt: Sie wird nicht geprüft, nur protokolliert. Jede Datei wird vor dem Löschen noch einmal per Prüfsumme kontrolliert und bleibt sonst liegen. Einen Probelauf gibt es mit Absicht nicht, sieh dir den Quarantäne-Ordner vorher selbst an.

Befehl: `hypersuite file purge <Ziel> --db <DB> --backup-confirmed "<Text>" [--older-than 30]`  
Alle Schalter: `hypersuite file purge --help`

**Sucht Dokumente nach Bedeutung statt Stichwort. Nach vielen neuen Dokumenten zuerst den Suchindex neu aufbauen.**  
Die Suche vergleicht die Bedeutung deines Suchtexts mit der der Dokumente und zeigt die nächsten Treffer (Standard: 10). Dafür braucht sie den Suchindex: Beim ersten Mal und wenn sich der Dokumentbestand deutlich geändert hat, setze das Häkchen und baue ihn neu auf. Das Lesen aller Dokumente kann bei großen Beständen lange dauern. Alles läuft lokal mit dem mitgelieferten Modell.

Befehl: `hypersuite file find "Suchtext" --db <DB>    (Index: hypersuite file find --rebuild --db <DB>)`  
Alle Schalter: `hypersuite file find --help`

**Hier entsteht die geordnete Bibliothek. Automatisch gewählt; „Ändern“ nimmt einen anderen Ordner.**  
Das Ziel ist der Ordner, in den später kopiert wird. Beim Planen wird dort nur ein Bericht unter .hyperfiler/plans/ abgelegt, sonst nichts. Am besten liegt das Ziel auf einer anderen Platte als die Quellen und hat genug freien Platz (er steht neben dem Feld). Dieselbe Platte ist erlaubt, es erscheint nur ein Hinweis. Die Quellen werden nie verändert: Ausführen kopiert nur.

Befehl: `hypersuite file plan <Ziel> --db <DB>`  
Alle Schalter: `hypersuite file plan --help`

**Welche Dateiarten geplant werden. „Sonstiges“ ist aus, bis du es einschaltest.**  
Fotos, Musik, Dokumente und Videos werden nach Art, Datum und Inhalt einsortiert. „Sonstiges“ (Installer, Archive, Dateien ohne erkennbare Art) wird nie stillschweigend mitgenommen, sondern nur, wenn du es einschaltest; es landet dann unverändert im Archiv. Weniger Arten bedeuten weniger zu lesen und ein schnelleres Planen.

Befehl: `hypersuite file plan <Ziel> --db <DB> --only photo,music,document,video`  
Alle Schalter: `hypersuite file plan --help`

**Die Index-Datenbank aus dem Scan. Sort liest sie nur; „Vorhandene öffnen…“ wählt eine andere.**  
Scan schreibt alles, was er gefunden hat (Pfad, Größe, Datum, Prüfsumme), in eine SQLite-Datei. Sort plant aus dieser Datei, ohne die Quellen erneut zu durchsuchen. „Zuletzt benutzt“ listet die letzten Datenbanken, „Neu anlegen“ gibt es nur in Scan. Bei sehr großen Datenbanken auf einer langsamen Platte erscheint die Dateizahl erst nach einer Weile („…“), Planen ist trotzdem sofort möglich. Das Kopieren der Datenbank auf eine SSD beschleunigt das Planen deutlich.

Befehl: `hypersuite index scan <Pfad> --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Schritt 1: entscheidet für jede Datei, wohin sie käme. Es wird nichts kopiert.**  
Planen liest die Datenbank und, bei Dokumenten, den Inhalt (Text, optional OCR und KI). Geschrieben wird nur der Bericht im Ziel und ein Eintrag pro Datei in der Datenbank. Schon gelesene Dokumente kommen aus dem Zwischenspeicher, ein abgebrochenes Planen geht dort weiter. Bei großen Beständen dauert es Stunden; „Später weitermachen“ hält es an, ohne das Gefundene zu verlieren.

Befehl: `hypersuite file plan <Ziel> --db <DB>`  
Alle Schalter: `hypersuite file plan --help`

**Schritt 2: zeigt, was der Plan vorhat und warum Dateien im Archiv landen. Liest nur.**  
Kontrollieren fasst den Plan zusammen (nach Art und Stand) und nennt Stichproben, warum Dateien in das Archiv („Inbox“) kamen. Das ist das Tor vor dem Kopieren: Erst wenn dir der Plan passt, geht es weiter. Der Bericht (Markdown und JSON) lässt sich über die Knöpfe daneben öffnen.

Befehl: `hypersuite file review --db <DB> <Plan-Nummer> <Ziel>`  
Alle Schalter: `hypersuite file review --help`

**Schritt 3: kopiert die Dateien ins Ziel und prüft jede Kopie. Quellen bleiben unberührt.**  
Ausführen kopiert jede geplante Datei in eine Zwischendatei, prüft die Prüfsumme und benennt sie erst dann um. Eine Quelle, die sich seit dem Planen geändert hat, schlägt fehl, statt still kopiert zu werden. Es ist gefahrlos unterbrechbar: Derselbe Plan setzt dort fort, wo er stand. Quellen werden nie verschoben oder gelöscht, das ist ein eigener, späterer Schritt („Quarantäne“).

Befehl: `hypersuite file apply --db <DB> <Plan-Nummer> <Ziel>`  
Alle Schalter: `hypersuite file apply --help`

**Schritt 4: prüft alle kopierten Dateien im Ziel noch einmal auf Unversehrtheit. Liest nur.**  
Prüfen berechnet die Prüfsumme jeder bereits bestätigten Kopie neu und vergleicht sie mit der beim Kopieren gespeicherten. So fallen Bitfehler oder später beschädigte Dateien auf. Es wird nichts repariert oder gelöscht; was damit geschieht, entscheidest du. Das Lesen des ganzen Ziels dauert bei großen Bibliotheken lange.

Befehl: `hypersuite file verify --db <DB> <Ziel>`  
Alle Schalter: `hypersuite file verify --help`

**Hält das Planen an. Das bisher Gelesene bleibt im Zwischenspeicher.**  
Der Knopf beendet den laufenden Plan. Gelesener Text und berechnete KI-Vektoren liegen im Zwischenspeicher (alle 200 Dokumente oder 30 Sekunden gesichert); höchstens diese letzten Sekunden gehen verloren. Beim nächsten „Plan erstellen“ kommt alles Gelesene von dort, das Planen geht also praktisch dort weiter, wo es stand. Der Plan sichert zuerst und beendet sich dann selbst (der Knopf zeigt „Wird angehalten …“); hängt er in einer Datei fest, wird er nach 20 Sekunden beendet.

Alle Schalter: `hypersuite file plan --help`

**Wie viele Dokumente gleichzeitig gelesen werden. Wirkt sofort, auch während des Planens.**  
Mehr Leser nutzen mehr Prozessorkerne und machen das Planen schneller, belasten den Rechner aber stärker. Der Standard ist die Hälfte der Kerne. Der Plan fällt bei jeder Zahl gleich aus. Der Regler schreibt die Zahl in eine Datei, die der laufende Plan neu liest (--jobs-file), du musst also nicht neu starten. Im Spiegel-Modus wird nichts gelesen, der Regler ist dort aus.

Befehl: `hypersuite file plan <Ziel> --db <DB> --jobs 8`  
Alle Schalter: `hypersuite file plan --help`

**Zeigt, wie stark der Prozessor ausgelastet ist und wie viel davon das Planen verbraucht.**  
Der äußere Wert ist die Auslastung des ganzen Rechners, der innere Teil gehört dem Planen samt seinen Hilfsprogrammen (OCR). Liegt der Zeiger weit unter dem Maximum, kannst du den Regler „Tempo“ erhöhen; ist der Rechner anderweitig ausgelastet, senke ihn.


**Eine Datei wird schon lange gelesen. Nach dem Zeitlimit kommt sie unverändert ins Archiv.**  
Manche Dateien (riesige oder beschädigte PDFs, lange OCR) brauchen ungewöhnlich lange. Nach dem Zeitlimit je Dokument (Advanced, Standard 120 Sekunden) wird die Datei nicht weiter gelesen, sondern landet mit dem Vermerk „zu lange gelesen“ im Archiv; das Planen läuft weiter. Mit 0 gibt es kein Limit, dann kann eine einzelne Datei das Planen sehr lange aufhalten.

Befehl: `hypersuite file plan <Ziel> --db <DB> --file-timeout 120`  
Alle Schalter: `hypersuite file plan --help`

**Setzt die Einstellungen von Sort auf die Standardwerte zurück.**  
Gilt nur für die Einstellungen in diesem Fenster (Ziel, Dateiarten, Modus, Dateien, OCR, KI, Zeitlimit, Tempo usw.). Weder Datenbank noch Pläne, Kopien oder Berichte werden verändert oder gelöscht.


**Welche Ordner durchsucht werden. Ohne eigene Wahl werden die Ordner deines Benutzers genommen.**  
Die Häkchen stehen für Ordner wie Dokumente, Bilder, Musik; „Ordner hinzufügen“ ergänzt beliebige weitere. Solange du nichts änderst, bleibt die Auswahl automatisch (Chip „Auto“). Scan liest nur Metadaten und Prüfsummen, ändert aber keine Datei. Der Scan merkt sich, was sich nicht geändert hat; wiederholte Läufe sind deshalb viel schneller.

Befehl: `hypersuite index scan <Pfad> [<Pfad> …] --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Ganze Laufwerke scannen. Fest eingebaute und angesteckte Laufwerke stehen zur Wahl.**  
Jedes Laufwerk, das Windows gerade kennt, erscheint als Chip mit freiem und gesamtem Platz im Hinweis. Wechsellaufwerke (USB) sind gekennzeichnet. Ein Laufwerk wird an seiner Seriennummer erkannt, nicht am Buchstaben: derselbe Stick gilt auch unter anderem Buchstaben als derselbe. Ist „Alle Laufwerke“ gesetzt (Advanced), ist diese Auswahl gesperrt.

Befehl: `hypersuite index scan E:\ F:\ --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Ordner, die nie betreten werden – samt allem darin. Voreingestellt sind sinnvolle Ausnahmen.**  
Die Chips sind Vorschläge: das Sort-Ziel, der hypersuite-Ordner, der Ordner der Datenbank, Rettungsordner und die Fotobibliothek – also Ordner, die hypersuite selbst anlegt und die nicht erneut gescannt werden sollen. Abwählen heißt: doch scannen. „Ordner ausschließen…“ nimmt weitere auf. Ein Ordner wird nicht einmal geöffnet, das spart Zeit und schützt vor gesperrten Ordnern. Namen wie node_modules schließt das Feld „Ausschließen“ in Advanced aus.

Befehl: `hypersuite index scan <Pfad> --exclude-dir <Ordner> --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Normal scannt wie gewohnt. Forensik ist für Laufwerke, die immer wieder ausfallen.**  
Der Forensik-Modus liest zuerst nur die Ordner und merkt sich, wo Dateien stehen, dann die Inhalte: kleine zuerst, defekte Stellen werden übersprungen. Fällt das Laufwerk aus (Hitze, wackeliges USB), pausiert der Scan, wartet die „Abkühlzeit“ ab (im Feld in Minuten, im Befehl in Sekunden) und macht allein weiter. Optional wird das USB-Gerät neu gestartet (nur mit Windows-Rückfrage). Es gibt keine Vorab-Zählung. Die Datenbank darf nicht auf dem gescannten Laufwerk liegen. Gerettete Dateien kopiert Sort („Rettung“).

Befehl: `hypersuite index scan <Pfad> --forensic --cooldown <Sekunden> --usb-restart --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Startet den Scan. Er liest nur und ändert keine Datei. Ein abgebrochener Scan lässt sich fortsetzen.**  
Vorher wird, wenn möglich, gezählt, damit Fortschritt und Restzeit stimmen („Ohne Zählen starten“ überspringt das). Danach steht neben dem Knopf, wie viel Platz die Datenbank etwa braucht und wie viel frei ist. Bricht der Scan ab (Fenster zu, Stromausfall), erscheint beim nächsten Öffnen eine Karte „Fortsetzen“; fertige Dateien werden nicht noch einmal angefasst.

Befehl: `hypersuite index scan <Pfad> --db <DB>      (fortsetzen: hypersuite index scan --resume --db <DB>)`  
Alle Schalter: `hypersuite index scan --help`

**Scannt jedes angeschlossene lokale Laufwerk statt einer Ordnerliste.**  
Praktisch für eine erste Bestandsaufnahme von allem, was gerade angesteckt ist. Netzlaufwerke bleiben außen vor, solange „Netzlaufwerke einbeziehen“ aus ist. Die Auswahl „Was scannen“ und „Laufwerke“ ist dann gesperrt.

Befehl: `hypersuite index scan --all-drives --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Nimmt bei „Alle Laufwerke“ auch Netzlaufwerke mit. Das kann sehr langsam sein.**  
Nur wirksam zusammen mit „Alle Laufwerke“. Ein Netzlaufwerk wird wie ein lokales Laufwerk gelesen; bei großen Freigaben dauert das lange, und die Prüfsummen laufen über das Netzwerk. hypersuite selbst sendet nichts; es greift nur auf Laufwerke zu, die du in Windows eingebunden hast.

Befehl: `hypersuite index scan --all-drives --include-network --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Folgt Verknüpfungen (Symlinks, Junctions) in andere Ordner. Standard: aus.**  
Aus ist sicher: Verknüpfungen, die im Kreis zeigen, würden sonst endlos laufen, und derselbe Inhalt würde mehrfach gezählt. Einschalten nur, wenn deine Daten wirklich über Verknüpfungen erreichbar sind.

Befehl: `hypersuite index scan <Pfad> --follow-symlinks --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Berechnet jede Prüfsumme neu, auch wenn Größe und Datum gleich sind. Dauert lange.**  
Normalerweise übernimmt ein erneuter Scan die gespeicherte Prüfsumme einer unveränderten Datei, das macht ihn schnell. Mit diesem Schalter wird alles neu gelesen. Sinnvoll, wenn du stille Datenfehler („Bitfäule“) vermutest, die Größe und Datum nicht verraten.

Befehl: `hypersuite index scan <Pfad> --rehash-all --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Online-Dateien (OneDrive, Nextcloud) überspringen oder herunterladen. Standard: überspringen.**  
„Überspringen“ merkt sich nur die Metadaten und öffnet die Datei nie, damit der Sync-Client nichts herunterlädt und sich nicht mit Fehlerfenstern meldet. „Herunterladen“ liest sie wie jede andere Datei: vollständige Prüfsummen, aber Zeit, Datenverkehr und lokaler Platz werden verbraucht, und ein kranker Sync-Client kann den Scan blockieren.

Befehl: `hypersuite index scan <Pfad> --cloud-files skip|hydrate --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Ordnernamen, die überall übersprungen werden, durch Komma getrennt.**  
Gilt für jeden Ordner dieses Namens, egal wo er liegt (Groß- und Kleinschreibung egal), im Gegensatz zu „Nicht scannen“, das einen bestimmten Ordner meint. Windows-Verwaltungsordner wie $RECYCLE.BIN und System Volume Information sind immer ausgeschlossen.

Befehl: `hypersuite index scan <Pfad> --exclude node_modules --exclude .git --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Wie viele Dateien gleichzeitig gelesen werden. Leer = automatisch.**  
Die Automatik passt sich dem Rechner an. Auf einer einzelnen, langsamen Festplatte bringen mehr Threads nichts und können das Lesen sogar verlangsamen; auf SSDs und Netzwerken helfen mehr.

Befehl: `hypersuite index scan <Pfad> --threads <Zahl> --db <DB>`  
Alle Schalter: `hypersuite index scan --help`

**Ordner für Berichte (Duplikate, Fotoplan usw.). Automatisch gewählt; „Öffnen“ zeigt ihn im Explorer.**  
Alle Berichte dieses Fensters landen als Markdown-Datei (und meist als JSON) in diesem Ordner. Sie enthalten Pfade deiner Dateien; gib sie nur weiter, wenn du das willst.

Befehl: `hypersuite index dupes --db <DB> -o <Datei.md>`  
Alle Schalter: `hypersuite index dupes --help`

**Kleinere Dateien werden bei der Duplikat-Suche ignoriert. Leer = alle.**  
Sehr kleine Dateien (Symbole, Konfigurationsdateien) sind zahlreich und selten interessant; eine Untergrenze macht den Bericht übersichtlich. Gleichheit heißt hier: gleiche Größe und gleiche Prüfsumme (BLAKE3) des ganzen Inhalts, nicht nur gleicher Name.

Befehl: `hypersuite index dupes --db <DB> --min-size <Bytes>`  
Alle Schalter: `hypersuite index dupes --help`

**Schreibt einen Bericht über doppelte Dateien aus allem, was je gescannt wurde. Löscht nichts.**  
Findet identische Inhalte über alle gescannten Laufwerke hinweg, auch über Sticks, die heute gar nicht angesteckt sind. Das Ergebnis ist ein Bericht (Markdown und JSON); aufräumen musst du selbst oder mit den späteren Schritten.

Befehl: `hypersuite index dupes --db <DB> -o hyperindex-report.md`  
Alle Schalter: `hypersuite index dupes --help`

**Zeigt, welche Ordner doppelte Inhalte enthalten – die Einheit, in der man aufräumt. Löscht nichts.**  
Statt einzelner Dateien listet der Bericht Ordner mit Anzahl, Größe und Datum der doppelten Inhalte. Er nutzt einen vorhandenen Duplikat-Bericht, wenn einer da ist, sonst rechnet er neu (--fresh erzwingt das).

Befehl: `hypersuite index doubles --db <DB> -o doubles.md`  
Alle Schalter: `hypersuite index doubles --help`

**Ermittelt das Aufnahmedatum und den Ort der Fotos aus den Dateien selbst. Nichts wird gesendet.**  
Reihenfolge der Quellen: EXIF-Aufnahmedatum, Datum im Dateinamen, Datum im Ordnernamen, zuletzt das Änderungsdatum der Datei (unsicher). Enthalten die Fotos GPS-Daten, wird der Ort über eine eingebaute Ortsdatenbank bestimmt, ohne Netzwerkzugriff. Ergebnisse werden gespeichert, ein erneuter Lauf kostet nur für neue Fotos etwas. „Neu berechnen“ erzwingt alles neu, etwa nach einem Programm-Update.

Befehl: `hypersuite index enrich --db <DB> [--force]`  
Alle Schalter: `hypersuite index enrich --help`

**Entwurf, wohin jedes Foto in eine datierte Bibliothek käme. Fasst keine Datei an.**  
Erzeugt plan.md und plan.json. Exakte Duplikate werden erkannt, Fotos ohne sicheres Datum kommen zur manuellen Sichtung in die Quarantäne. Das Dateisystem bleibt unberührt; erst „Ausführen“ kopiert. Dies ist der Foto-Plan von Scan; der umfassende Plan für alle Dateiarten steht in Sort.

Befehl: `hypersuite index plan --db <DB> -o plan.md`  
Alle Schalter: `hypersuite index plan --help`

**Ordner, unter dem die sortierte Fotobibliothek entsteht.**  
Die Zielpfade des Plans sind relativ und werden hier eingesetzt. Wähle einen Ordner mit genug freiem Platz, am besten auf einer anderen Platte als die Quellen.

Befehl: `hypersuite index apply --plan plan.json --library-root <Ordner> --db <DB>`  
Alle Schalter: `hypersuite index apply --help`

**Kopiert die Fotos laut Plan in die Bibliothek und prüft jede Kopie. Die Quelle bleibt unberührt.**  
Jeder Versuch wird protokolliert, ein unterbrochener Lauf lässt sich gefahrlos wiederholen. Der „Testlauf“ zeigt nur, was passieren würde, und schreibt nichts. Ohne Testlauf musst du bestätigen, dass der Vorgang ausgeführt werden soll. Gelesen wird plan.json, nicht die .md-Datei.

Befehl: `hypersuite index apply --plan plan.json --library-root <Ordner> [--dry-run] --db <DB>`  
Alle Schalter: `hypersuite index apply --help`

**Macht einen Lauf rückgängig: löscht nur die Dateien, die dieser Lauf selbst angelegt hat.**  
Die Auftragsnummer steht am Ende jedes Laufs und in dessen JSON-Bericht. Ohne „Wirklich löschen“ werden die betroffenen Dateien nur aufgelistet. Quellen werden nie gelöscht, nur die Kopien im Ziel.

Befehl: `hypersuite index apply --undo <Auftrag> [--force] --db <DB>`  
Alle Schalter: `hypersuite index apply --help`

**Reduziert doppelte Musik auf eine Kopie je Titel, bevor man sie in beets importiert. Löscht nichts.**  
Derselbe Titel auf mehreren Sicherungsplatten wird einmal aufgeführt, damit beets die Online-Suche nicht mehrfach bezahlt. beets selbst wird nicht gestartet, nichts wird verschoben oder gelöscht; beets bleibt das Werkzeug, das die Musik ordnet und beschriftet.

Befehl: `hypersuite index prefilter --db <DB> -o beets-import.md`  
Alle Schalter: `hypersuite index prefilter --help`

**Schaut in die Datenbank: Laufwerke, Gesamtzahlen und aufgezeichnete Pläne. Nur Lesen.**  
„Laufwerke“ listet jedes je gescannte Laufwerk mit Seriennummer, auch nicht angesteckte. „Zahlen“ zeigt Gesamtwerte, letzte Scans und unterbrochene Scans. „Aktionen“ zeigt die Pläne und ihren Stand; mit einer Plan-Nummer die einzelnen Aktionen. Nichts davon ändert etwas.

Befehl: `hypersuite index volumes|stats|actions --db <DB>`  
Alle Schalter: `hypersuite index --help`

**Setzt die Einstellungen von Scan auf die Standardwerte zurück.**  
Betrifft nur die Einstellungen dieses Fensters. Die Datenbank, Berichte und gescannte Daten bleiben, wie sie sind.


**Die Outlook-Datei (.pst), die übernommen wird. Sie wird nur gelesen, nie verändert.**  
„Durchsuchen“ wählt eine Datei; gefundene Kandidaten stehen in der Liste daneben. hypersuite öffnet die PST streng lesend, ohne Outlook. Ob die Datei lesbar ist und wie viele Ordner und Nachrichten sie enthält, steht im Hinweis darunter oder unter „Inhalt prüfen“.

Befehl: `hypersuite mail inspect <PST-Datei>`  
Alle Schalter: `hypersuite mail --help`

**Ziel der Mails: ein Thunderbird-Profil oder ein eigener Ordner. Das Profil wird vorher gesichert.**  
Bei einem Profil prüft hypersuite, dass Thunderbird geschlossen ist, sichert das Profil, wandelt die Mails um, prüft das Ergebnis und kopiert erst dann in die „Lokalen Ordner“. Dafür musst du bestätigen, weil dein lebendes Profil verändert wird. „Ändern“ wählt ein anderes Profil, wenn es mehrere gibt. Der mbox-Weg (Advanced) berührt Thunderbird nicht.

Befehl: `hypersuite mail auto <PST-Datei> --profile <Profil>`  
Alle Schalter: `hypersuite mail auto --help`

**Übernimmt die Mails in Thunderbird. Vorher gibt es eine Sicherung und eine Rückfrage.**  
Der Ablauf ist geführt: Thunderbird geschlossen? Sicherung des Profils, Umwandlung, Prüfung, Kopie. Mit „Testlauf“ (Advanced) wird alles außer der Änderung des Profils gemacht. Die PST-Datei bleibt unverändert. Der Schalter -y im Befehl beantwortet alle Rückfragen mit Ja (nötig ohne Terminal); in der Oberfläche ersetzt ihn die Bestätigung.

Befehl: `hypersuite mail auto <PST-Datei> --profile <Profil> [--overwrite] [--dry-run] -y`  
Alle Schalter: `hypersuite mail auto --help`

**Thunderbird-Profil: direkt hineinschreiben. mbox-Ordner: nur Dateien erzeugen, Thunderbird unberührt.**  
Mit dem mbox-Ordner entsteht eine eigenständige Ordnerstruktur im Thunderbird-Format, die du selbst einbinden oder archivieren kannst. Das ist der risikoärmste Weg, weil kein bestehendes Profil verändert wird. Das Profil kann auch im Befehl `mail export` (ohne Profil) gewählt werden.

Befehl: `hypersuite mail auto <PST> --profile <Profil>      |      hypersuite mail export <PST> --output <Ordner>`  
Alle Schalter: `hypersuite mail --help`

**Packt alles unter einen Oberordner, damit mehrere PSTs ihre „Posteingang“-Ordner nicht vermischen.**  
Ohne Oberordner würden zwei PST-Dateien im selben Profil ihre gleichnamigen Ordner (Posteingang, Gesendet) zusammenwerfen. Leer lassen heißt: Name der PST-Datei. Im Befehl bedeutet --root-name "" ebenfalls den Dateinamen.

Befehl: `hypersuite mail auto <PST> --root-name "<Name>"`  
Alle Schalter: `hypersuite mail auto --help`

**Erlaubt, vorhandene Postfächer oder Ordner mit gleichem Namen zu ersetzen. Standard: aus.**  
Ohne den Schalter bricht die Übernahme ab, statt etwas Vorhandenes zu überschreiben. Einschalten nur, wenn du genau das willst, etwa um einen früheren, unvollständigen Versuch zu ersetzen.

Befehl: `hypersuite mail auto <PST> --overwrite`  
Alle Schalter: `hypersuite mail auto --help`

**Probelauf: macht alles außer dem Schreiben ins Profil und zeigt, was passieren würde.**  
Gut als erster Versuch bei einer großen PST. Das Profil wird nicht verändert und es gibt keine Rückfrage zum Profil. Hat der Testlauf Fehler gemeldet, sind sie vor dem echten Lauf zu klären.

Befehl: `hypersuite mail auto <PST> --dry-run`  
Alle Schalter: `hypersuite mail auto --help`

**Startet Thunderbird nach der Übernahme. Nur beim Profil-Ziel.**  
Praktisch, um das Ergebnis gleich zu prüfen. Im Befehl ist es umgekehrt: --no-start verhindert den Start.

Befehl: `hypersuite mail auto <PST> --no-start`  
Alle Schalter: `hypersuite mail auto --help`

**Liest Ordnerstruktur und Nachrichtenzahlen der PST. Schreibt nichts.**  
Ein schneller Test, ob die Datei lesbar ist, bevor du übernimmst. Beschädigte oder passwortgeschützte PSTs fallen hier auf.

Befehl: `hypersuite mail inspect <PST-Datei>`  
Alle Schalter: `hypersuite mail inspect --help`

**Setzt die Optionen von Mail auf die Standardwerte zurück. Die gewählte PST bleibt.**  
Betrifft nur Einstellungen dieses Fensters. Weder Thunderbird noch bereits übernommene Mails werden angefasst.


**Entpackt die eingebauten Werkzeuge (KI-Modell, PDF, OCR, Audio) in einen lokalen Ordner.**  
Alles, was hypersuite braucht, steckt in der Exe und wird beim ersten Gebrauch unter %LOCALAPPDATA%\hypersuite\runtime entpackt. Es wird nichts heruntergeladen und nichts gesendet. Jede entpackte Datei wird gegen eine Prüfsumme geprüft.

Befehl: `hypersuite tools`  
Alle Schalter: `hypersuite tools --help`

**Prüft jede entpackte Datei gegen ihre SHA-256-Prüfsumme.**  
Zeigt, ob eine Datei beschädigt wurde oder fehlt, etwa nach einem Festplattenfehler oder wenn ein Virenscanner eingegriffen hat. Bei einem Fehler hilft „Neu entpacken“.

Befehl: `hypersuite tools --verify`  
Alle Schalter: `hypersuite tools --help`

**Löscht die entpackte Kopie der Werkzeuge und entpackt sie neu. Eigene Daten bleiben.**  
Betroffen ist nur der Entpack-Ordner (Anzeige „Entpackt nach“). Datenbanken, Pläne, Berichte und der Zwischenspeicher liegen woanders und bleiben unberührt. Das Neuentpacken dauert wenige Sekunden.

Befehl: `hypersuite tools --reset`  
Alle Schalter: `hypersuite tools --help`

**Zeigt, ob die eingebauten Werkzeuge bereit sind. Grün = alles entpackt und nutzbar.**  
Die Werkzeuge (KI-Modell, PDFium, Tesseract, fpcalc) sind in der Exe enthalten. Ein Klick öffnet die Detailansicht mit Prüfen und Neu entpacken. Das Programm hat keine Netzwerkfunktion und sendet nichts.

Befehl: `hypersuite tools`  
Alle Schalter: `hypersuite tools --help`

