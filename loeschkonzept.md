# Löschkonzept für das Mailarchiv: Vorlage

**Büro:** [Name des Büros] · **Gültig ab:** [Datum] · **Verantwortlich:**
[Archiv-Admin] · **Stellvertretung:** [Name] · **Fassung:** 1

Vorlage von Filum, Stand 24.08.2026, nachgeführt 26.09.2026, nach dem Gerüst der DIN 66398
(Leitlinie Löschkonzept). Die eckigen Klammern füllt das Büro aus; was ohne
Klammern dasteht, beschreibt, wie das Archiv tatsächlich arbeitet. Keine
Rechtsberatung. Bei Zweifelsfällen entscheidet das Büro mit seiner
Rechtsberatung, nicht die Software.

## 1. Zweck

Das Datenschutzrecht verlangt beides zugleich: aufbewahren, was gebraucht
wird, und vernichten oder anonymisieren, was nicht mehr erforderlich ist
(DSG Art. 6 Abs. 4: eine Pflicht, keine Option). Dieses Konzept legt fest,
WER im Mailarchiv WANN WAS löscht, und wie das nachweisbar bleibt. Es
gehört zur Verfahrensdokumentation und wird wie sie aufbewahrt.

## 2. Rollen

| Rolle | Wer | Darf |
|---|---|---|
| Archiv-Admin | [Name] | löschen (über die Löschfunktion, nie im Dateisystem), Sperren setzen und aufheben, Fristen pflegen, Snapshots verwalten und Dateien daraus zurückholen (Beilage 1) |
| Stellvertretung | [Name] | dasselbe, bei Abwesenheit |
| Belegschaft | alle | archivieren und lesen. Löschen und ändern könnte sie im Archiv technisch, darf es aber nicht; was fehlt oder verändert ist, meldet die Prüfung, und zurück kommt es aus dem Snapshot (Beilage 1) |

Empfehlung Vier-Augen: Löschungen auf Verlangen Dritter stellt eine Person
als Antrag zusammen (Trefferliste aus «Auskunft und Löschung»), die andere
führt aus. Beide Namen gehören in den Grund.

## 3. Datenarten und Löschklassen

Ein Projektordner enthält Verschiedenes, und Verschiedenes hat
verschiedene Fristen:

| Klasse | Beispiele | Regelfrist | Grundlage |
|---|---|---|---|
| Buchungsrelevante Korrespondenz | Honorarabrechnungen, Zahlungsfreigaben, Belege zu Buchungen | 10 Jahre ab Ablauf des Geschäftsjahrs | OR 958f Abs. 1, gesetzliche Pflicht |
| Übrige Projektkorrespondenz | Planlieferungen, Absprachen, Warnungen, Protokolle | [Abschluss + 10 Jahre] | GESCHÄFTSENTSCHEID, keine gesetzliche Pflicht, bemessen an Verjährung und Mängelrechten (OR 127; OR 371 Abs. 2: fünf Jahre ab Abnahme, seit 2026 nicht mehr zulasten des Bestellers abkürzbar) |
| Nicht Projektbezogenes im Archiv | Bewerbungen, abgesprungene Interessenten, Einsprechende | kurz, [z.B. 6 Monate nach Erledigung] | DSG 6 Abs. 4: nicht mehr erforderlich = weg |
| Irrtümlich Archiviertes / Privates | private Mails von Mitarbeitenden | sofort nach Feststellung | Art. 328b OR, Verhältnismässigkeit; Privates gehört nie ins Geschäftsarchiv (siehe Ziff. 8) |

Wer selbst unbewegliche Gegenstände hält oder baut, prüft zusätzlich die
20-Jahre-Frist des MWSTG Art. 70 Abs. 3 (Einlageentsteuerung /
Eigenverbrauch EIGENER Immobilien. Sie trifft die steuerpflichtige Person,
nicht die Projektkorrespondenz über fremde Bauten).

## 4. Fristen je Projekt

Die Frist lebt IM Archiv, nicht in einer Nebenliste: Auf der Projektseite
(Abschnitt «Aufbewahrung») trägt der Archiv-Admin den **Projektabschluss**
ein (die Abnahme, nicht das letzte Kalenderjahr) und die **Jahre**
(Vorgabe zehn). Das Archiv rechnet den Ablauf auf den Kalendertag und sagt
seinen Zustand selbst: *offen*, *läuft bis …*, *abgelaufen, prüfen*.

Regel des Büros: [z.B. «Abschluss = Datum der Abnahme laut Protokoll;
Jahre = 10; länger nur mit dokumentiertem Grund».]

## 5. Der jährliche Durchgang

Einmal im Jahr, [z.B. jeweils im Januar], zusammen mit der
Archivprüfung, geht der Archiv-Admin die Projekte durch:

1. In der App «Jahresdurchgang …» öffnen. Er zeigt alle Projekte auf einen
   Blick, geordnet nach *abgelaufen*, *gesperrt*, *läuft* und *offen*. Ein
   Projekt, dessen Ablage beim Durchgang nicht erreichbar war, steht mit
   diesem Hinweis unter *offen*.
2. Je abgelaufenes Projekt ENTSCHEIDEN und den Entscheid festhalten:
   * **Löschen** über «Auskunft und Löschung», mit Grund
     («Aufbewahrungsfrist abgelaufen, Durchgang [Jahr]»).
   * **Verlängern**: Jahre anpassen, Grund hier notieren:
     [Tabelle/Anhang].
3. Den Durchgang als Bericht sichern («Jahresdurchgang [Datum].txt») und
   das Prüfprotokoll der Jahresprüfung ablegen lassen (geschieht
   automatisch unter `.filum/pruefungen/`).

Die Software entscheidet nie selbst: im Jahresdurchgang wird nichts
gelöscht, er zeigt und protokolliert.

## 6. Begehren betroffener Personen

**Auskunft:** DSG Art. 25, in der Regel innert 30 Tagen (für Kunden im
DSGVO-Bereich: Art. 12 Abs. 3, ein Monat). Werkzeug: «Auskunft und
Löschung» sucht eine Adresse in Von/An/Cc/Bcc UND als Erwähnung im Text.
Die Textsuche findet nur wörtliche Nennungen. Diese Grenze wird der
betroffenen Person mitgeteilt, statt Vollständigkeit vorzutäuschen.

**Löschung:** Zuerst die Gegenprüfung. Eine gesetzliche
Aufbewahrungspflicht geht vor (DSG 31 Abs. 1; DSGVO Art. 17 Abs. 3 lit. b),
ebenso laufende Rechtsansprüche (lit. e) und eine gesetzte Löschsperre.
Was keiner Pflicht unterliegt (Bewerbungen, Einsprechende, blosse
Erwähnungen), wird gelöscht. Jede Löschung braucht einen Grund und
hinterlässt einen Vermerk (Ziff. 9). Antwort an die Person: was gelöscht
wurde, was aufgrund welcher Pflicht (noch) nicht, und bis wann die
Nachricht noch in den Sicherungen liegt (Ziff. 10).

## 7. Löschsperre (laufende Verfahren)

Bei einem laufenden oder konkret absehbaren Verfahren setzt der
Archiv-Admin auf der Projektseite die **Löschsperre**, mit Grund
(«[Verfahren/Geschäftsnummer]»). Ab dann verweigert das Archiv JEDE
Löschung, auch dem Admin, bis die Sperre mit Grund wieder aufgehoben wird.
Setzen und Aufheben stehen dauerhaft im Sperr-Protokoll des Archivs
(Person, Zeitpunkt, Grund). Wer Sperren setzt und aufhebt: [Archiv-Admin;
auf Weisung von …].

## 8. Private Mails

Privates gehört nicht ins Geschäftsarchiv. Filum archiviert nur, was in
die Projektordner einsortiert wurde. Privates landet also nur irrtümlich
im Archiv und wird nach Feststellung gelöscht, Grund «irrtümlich
archiviert / privat». Massgebend ist das Nutzungsreglement des Büros
[Beilage 2]; besteht keines, ist es zu erlassen.

## 9. Nachweis

* **Der Löschvermerk.** Jede Löschung ersetzt die Nachricht durch einen
  Vermerk im Ordner der Originale. Er heisst nach der Kennung der Nachricht
  (`<Kennung>.geloescht.json`), derselben, die in der Löschliste steht
  (Ziff. 10); ihre ersten acht Zeichen standen im Dateinamen der Nachricht
  direkt vor `.eml`. Der Vermerk hält fest, WAS entfernt wurde (beide
  Prüfkennungen und die Prüfsummen der Anhänge, also Hashes, kein Inhalt),
  WANN, durch WEN und aus welchem GRUND. Die Lücke bleibt in Übersicht und
  Verlauf sichtbar und benannt, mit Datum und Richtung. Absendername und
  Betreff gehen mit der Nachricht: Sie standen auch in ihrem Dateinamen, und
  darum trägt weder der Vermerk noch der geschwärzte Eintrag noch der
  Archivstand diesen Namen weiter. Text und Adressen
  sind überall entfernt, auch aus dem Suchindex. Anhänge gehen mit, soweit keine andere
  Nachricht sie hat: Filum entfernt im Ordner des Anhangs jede Datei mit
  genau seinem Inhalt, auch eine Kopie unter anderem Namen, und lässt jede
  andere Datei liegen, auch die eines Anhangs, den eine andere Nachricht
  braucht. Liegt im Ablageordner auf dem Weg zu einer Datei, die die
  Löschung anfassen müsste, ein Verweis (symbolischer Link), entfernt Filum
  nichts und sagt es. Liegt die
  Nachricht als Gerüst (Option «Anhänge nur einmal ablegen»), gilt für
  seine Teile dasselbe. Kann Filum
  einen Teil des Archivs nicht lesen, den die Löschung braucht, entfernt es
  nichts und sagt es. Bricht eine Löschung ab, solange das Original oder
  ein Anhang, der mit ihm gehen muss, noch daliegt, nennt die Prüfung sie
  «Löschung nicht vollzogen». Lässt sich das gerade nicht lesen oder gilt
  der Löschvermerk nicht mehr, nennt sie die Löschung «nicht bestätigt»,
  je mit eigenem Satz: Was niemand gesehen hat, behauptet Filum nicht. Alle
  drei lassen sich
  dann in «Auskunft und Löschung» erneut wählen, und Filum führt sie samt
  Anhängen zu Ende, solange ihr Löschvermerk unverändert daliegt; gilt er
  nicht mehr, entfernt Filum nichts und sagt, dass der Vermerk aus der
  Sicherung zurückzuholen ist.
* **Die Prüfung unterscheidet.** Die Archivprüfung (in der App, oder ohne
  Filum mit `python3 -I .filum/pruefen.py`, unter Windows
  `py -3 -I .filum/pruefen.py`) kennt drei Ergebnisse: vorhanden,
  **entfernt mit Vermerk** (in Ordnung) und fehlend ohne Vermerk (Alarm).
  Fehlt einer Löschung der Vermerk oder der geschwärzte Eintrag, nennt sie
  das eigens (Alarm); zurückgeholt wird dann dieses Stück, nie die
  Nachricht (Beilage 1). Eine dokumentierte Löschung ist damit von einer Manipulation
  unterscheidbar, und zwar für Dritte nachrechenbar.
* **Ablage der Protokolle.** Prüfprotokolle unter `.filum/pruefungen/`,
  Sperr-Protokoll im Archivstand, dieses Konzept samt Beilagen bei der
  Verfahrensdokumentation. Aufbewahrung wie die Daten selbst (GeBüV
  Art. 4 Abs. 2 sinngemäss).

## 10. Sicherungen

Das NAS sichert das Archiv-Share automatisch (Snapshots, dazu [eine Kopie
ausser Haus]); Einrichtung und Wiederherstellen beschreibt Beilage 1. Für
das Löschen heisst das:

* **Eine gelöschte Nachricht bleibt in den Sicherungen**, bis die letzte
  Sicherung abläuft, die sie noch enthält: im Archiv-Share nach
  24 Monaten, in der Kopie ausser Haus nach [Frist]. Die 24 Monate sind
  der Richtwert aus Beilage 1; das Büro kann ihn anpassen und trägt dann
  seinen Wert hier ein. Einzeln daraus
  löschen lässt sie sich nicht. Die Sicherungen sind für die Belegschaft
  unzugänglich, werden für nichts anderes verwendet und nach diesem Plan
  überschrieben.
* **Zurückgeholt wird nur einzeln**, was die Prüfung als fehlend oder
  verändert nennt, und nie eine gelöschte Nachricht: Liegt im jüngsten
  Snapshot im Ordner der Originale ein Vermerk, dessen Name mit den acht
  Zeichen vor `.eml` im Dateinamen der Nachricht beginnt, bleibt sie weg,
  und fehlt nur der Vermerk, kommt nur er zurück. Die Dateien unter
  `.filum/stand` kommen nur aus Sicherungen nach der letzten Löschung
  zurück, weil ältere den Inhalt gelöschter Nachrichten tragen.
* **Nach einer Gesamtwiederherstellung** (ganzes Share aus einer älteren
  Sicherung) kennt das Archiv die Löschungen seit dieser Sicherung nicht
  mehr. Der Archiv-Admin wiederholt sie anhand der **Löschliste**
  (Beilage 4), die ausserhalb des Archivs geführt wird: je Löschung Datum,
  Projekt, Grund und die Kennungen der entfernten Nachrichten. Den Eintrag
  dafür zeigt Filum nach jeder Löschung unter «Für die Löschliste» zum
  Übertragen (die Kennung steht auch als `contentId` im Vermerk). Zum
  Wiederholen sucht der Archiv-Admin in «Auskunft und Löschung» über alle
  Projekte nach **Kennung** und fügt die Kennungen aus der Liste ein, auch
  den ganzen Eintrag samt Datum und Grund, nicht aber den Vermerk selbst.
  Filum findet genau diese Nachrichten, zeigt schon entfernte als erledigt,
  nennt Löschungen, die begonnen, aber nicht vollzogen sind, und Kennungen,
  die in keinem durchsuchten Projekt liegen. Durchsucht werden nur
  Projekte, deren Ablage auf diesem Rechner verbunden ist (Beilage 1,
  «Nach einer Gesamtwiederherstellung»). Das trägt auch Löschungen ohne
  Begehren (Privatmail, abgelaufene Frist), zu denen es keine Adresse gibt.
  Keine Adresse der Person in der Liste, auch nicht im Grund: Wer ein
  Begehren gestellt hat, belegt der Schriftverkehr dazu. Steht im Grund
  eine Mailadresse, weist Filum vor dem Entfernen darauf hin. Betreff und
  Dateiname gehören ebenso wenig hinein: Die Liste liegt ausserhalb des
  Archivs und hält vom Gelöschten nichts fest. Die wiederholte Löschung
  trägt im Vermerk ihren eigenen Zeitpunkt; die Verfahrensdokumentation im
  Archiv sagt, dass ein Löschstempel, der später liegt als die ursprüngliche
  Löschung, dann kein Widerspruch ist.

Grundlage: DSG Art. 6 Abs. 4; Europäischer Datenschutzausschuss, Bericht
zur koordinierten Prüfung des Rechts auf Löschung (Februar 2026),
Abschnitt 4.2.6: Löschbegehren festhalten und auf wiederhergestellten
Systemen umsetzen.

## 11. Beilagen

1. Backup-Vorgabeblatt (Einrichtung des Archiv-Shares, Snapshots, Wiederherstellen)
2. Nutzungsreglement E-Mail/Privatnutzung des Büros
3. [Fristen-/Entscheidliste des jährlichen Durchgangs]
4. [Löschliste: je Löschung Datum, Projekt, Grund und die Kennungen der
   entfernten Nachrichten (`contentId`), übertragen aus «Für die
   Löschliste» in Filum; keine Adresse, kein Betreff]

*Vorlage: Filum/bimover, 24.08.2026. Keine Rechtsberatung; Normstände:
DSG/OR/GeBüV per 2026, DSGVO für Kunden im EU-Bereich.*
