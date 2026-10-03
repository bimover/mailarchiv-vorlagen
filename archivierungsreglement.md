# Archivierungsreglement für das Mailarchiv: Vorlage

Was archiviert wird, wo es liegt, wer darauf zugreift und wie lange es
bleibt. Das Gegenstück zum Nutzungsreglement.

Stand 26.09.2026. Vorlage von Filum, nach DSG, DSV und der Praxis des EDÖB.
Die eckigen Klammern füllt das Büro aus; was ohne Klammern dasteht,
beschreibt, wie das Archiv tatsächlich arbeitet. Keine Rechtsberatung.

---

**Büro:** [Name des Büros] · **Gültig ab:** [Datum] · **Verantwortlich für
das Archiv:** [Name] · **Stellvertretung:** [Name] · **Fassung:** 1

## 1. Zweck des Archivs

Das Büro archiviert Projektkorrespondenz, damit sie den Lebenszyklus eines
Postfachs überdauert. Gebraucht wird sie für die Fortführung laufender
Projekte, für die Rechenschaft gegenüber der Bauherrschaft (OR Art. 400
Abs. 1) und für die Dauer der Haftung aus Werkvertrag und Auftrag.

Das Archiv ist kein Überwachungssystem und wird nicht zur Leistungs- oder
Verhaltenskontrolle verwendet.

## 2. Was archiviert wird und was nicht

| Was | Im Archiv |
|---|---|
| Nachrichten, die eine Person selbst in den Projektordner eines Projekts einsortiert hat | ja |
| Nachrichten aus Posteingang und Gesendet, die eine Regel der Person oder ihr eigener Entscheid einem Projekt gibt | ja |
| Die Anhänge dieser Nachrichten | ja |
| Nachrichten von Adressen und Domains, die die Person als privat bezeichnet | nein, in keinem Projekt |
| Alles Übrige im Postfach | nein |
| Der öffentliche Schlüssel, mit dem eine Absenderdomäne ihre Nachrichten unterschreibt | ja, soweit eine archivierte Nachricht ihn nennt |
| Der Ordner «Privat» | nein, er wird nie als Quelle gewählt |
| Entwürfe | nein, sie werden übersprungen |
| Teams-Chats, SMS, WhatsApp | nein, nicht erfasst |

Was ins Archiv kommt, hat eine Person durch Einsortieren oder durch ihre
Regeln dazu bestimmt. Um die Regeln anzuwenden, liest Filum auf ihrem
Rechner Posteingang und Gesendet samt dem Text neuer Nachrichten; was zu
mehreren Projekten passt, legt es nur ihr zur Entscheidung vor. Stimmt sie
zu, archiviert Filum ihre Projekte danach alle zwei Stunden von selbst,
solange sie am Rechner angemeldet ist; abschalten kann sie das jederzeit in
den Einstellungen. Das übrige Postfach archiviert Filum nie.

Für die öffentlichen Schlüssel holt Filum im Hintergrund die Kopfzeilen der
neuesten Nachrichten im Posteingang, ohne Text und ohne Anhänge. Ausgewertet
wird davon nur die Zeile, mit der eine Absenderdomäne ihre Nachricht
unterschreibt; den Schlüssel fragt Filum über den Namensdienst des Büros ab.
Die Schlüssel liegen bis zu zwölf Monate in einem Vorrat auf dem Rechner;
ins Archiv kommen nur die, die eine archivierte Nachricht nennt.

## 3. Wo das Archiv liegt

Ablageort: [Pfad, zum Beispiel `\\nas\Mailarchiv` oder `/Volumes/Mailarchiv`]

Das Archiv liegt auf einem Träger des Büros. Es wird keine Kopie bei einem
Anbieter gehalten, und die Inhalte werden nicht an Dritte übermittelt. Was
Filum an bimover meldet, sind Zahlen und Hashwerte für die Lizenz, keine
Inhalte (Ziffer 10).

Das Archiv liegt in einem eigenen Share, getrennt von der Projektablage
(GeBüV Art. 7 verlangt die Trennung des Archivs vom laufenden Bestand).

## 4. Wer Zugriff hat

| Rolle | Wer | Darf |
|---|---|---|
| Alle Mitarbeiter | [Gruppe] | archivieren, lesen |
| Archiv-Verantwortung | [Name] | zusätzlich: löschen über die App, Sperren setzen, Fristen pflegen |
| Stellvertretung | [Name] | dasselbe bei Abwesenheit |
| NAS-Verwaltung | [Name oder Dienstleister] | Sicherungen verwalten und zurückspielen |

Berechtigungen je Projekt gibt es nicht. Wer im Büro arbeitet, sieht das
Archiv des Büros. Diese Entscheidung ist bewusst: Eine Rechtematrix über
alle Projekte wäre nach kurzer Zeit nicht mehr gepflegt und damit falsch.

Technisch könnte jede Person im Archiv Dateien ändern oder löschen. Erlaubt
ist es nicht. Jede Abweichung fällt bei der Prüfung auf, und die Sicherung
des NAS bringt zurück, was fehlt.

## 5. Sicherheit

| Ziel (DSV Art. 2) | Womit erreicht |
|---|---|
| Vertraulichkeit | Zugriff nur über die persönlichen Konten, kein geteiltes Archivkonto, Share nur im Büronetz |
| Verfügbarkeit | tägliche Sicherungen des NAS, aufbewahrt [Dauer], Rückspielen getestet am [Datum] |
| Integrität | Prüfwert je Nachricht, Beleg über den ganzen Bestand, verkettet und von einem Dritten zeitgestempelt |
| Nachvollziehbarkeit | Protokoll je Lauf und je Prüfung, Vermerk bei jeder Löschung |

Die Zugriffe auf das Share zeichnet das NAS auf: [ja, seit Datum / noch
einzurichten]. GeBüV Art. 8 verlangt das für ein Archiv.

## 6. Wie lange

Die Frist steht je Projekt im Archiv selbst, nicht in einer Nebenliste.
Beginn ist der Projektabschluss, also die Abnahme, nicht das Kalenderjahr.

Regel des Büros: [Vorschlag: zehn Jahre ab Abnahme; länger nur mit
dokumentiertem Grund.] Die Klassen und ihre Fristen stehen im Löschkonzept
(`loeschkonzept.md`), das zu diesem Reglement gehört.

Einmal im Jahr, im [Monat], geht die Archiv-Verantwortung alle Projekte
durch und hält den Durchgang schriftlich fest.

## 7. Löschen

Gelöscht wird nur über die App, nie im Dateisystem. Die Löschung entfernt
die Nachricht und ihre Lesefassung, schwärzt die Angaben in der Satzdatei
und hinterlässt einen Vermerk mit Zeitpunkt, Person und Grund. So bleibt
unterscheidbar, was rechtmässig gelöscht wurde und was fehlt.

Läuft oder droht ein Verfahren, setzt die Archiv-Verantwortung vorher die
Löschsperre. Sie blockiert jede Löschung, bis sie wieder aufgehoben wird,
und beides wird festgehalten.

## 8. Wenn eine private Nachricht im Archiv landet

Wer bemerkt, dass eine private Nachricht versehentlich archiviert wurde,
meldet das [Name]. Sie wird entfernt, ohne dass jemand ihren Inhalt liest,
und die Entfernung wird wie jede Löschung vermerkt. Die betroffene Person
wird informiert.

## 9. Auskunft

Verlangt jemand Auskunft über seine Daten (DSG Art. 25), gilt:

1. [Name] nimmt das Begehren entgegen und hält Eingangsdatum fest. Die
   Auskunft ist in der Regel innert 30 Tagen zu erteilen.
2. Gesucht wird in «Auskunft und Löschung» nach der Mailadresse der Person.
3. Vor der Herausgabe wird geprüft, welche Angaben Dritte betreffen. Ein
   Gesprächsverlauf enthält fast immer Daten anderer Personen; er wird nicht
   ungeprüft herausgegeben (DSG Art. 26 Abs. 1 lit. b).
4. Die Auskunft nennt auch die Aufbewahrungsdauer und die Empfänger, an die
   Daten gehen.

## 10. Was an bimover geht

Für die Lizenz fragt die App vor jedem Lauf mit einem Hashwert je Postfach,
aus dem archiviert wird, statt der Adresse. Nach dem Lauf meldet sie
dieselben Hashwerte, eine Kennung des Archivs ohne Projektnamen und ohne
Adresse, Kennung und Zeitpunkt des Laufs, die Prüfsumme des jüngsten Belegs,
die Zahl der Nachrichten und die Zahl der Belege. Der Hashwert ist pseudonym: Wer
die Adresse kennt, kann ihn nachrechnen. Inhalte, Betreffzeilen und Adressen
der Korrespondenz gehen nicht hinaus.

Wer Filum mit einem bimover-Konto verbindet, gibt dabei Name, Mailadresse
und die Kennungen von Microsoft an bimover, dazu den Namen des Rechners.

Ein Diagnosebericht geht nur hinaus, wenn eine Person ihn ausdrücklich
freigibt. Er enthält weder Betreff noch Adressen der Korrespondenz, wohl
aber ihre eigene Kontoadresse, Projektname, Projektnummer und den letzten
Ordner des Ablagepfads.

Ausserhalb von bimover erhalten der Zeitstempeldienst je Beleg einen Hash
und der Namensdienst des Büros die Domäne eines Absenders, deren Schlüssel
Filum abfragt. Eine Adresse oder einen Inhalt erhält keiner der beiden.

Die Mitarbeiter sind darüber informiert (DSG Art. 19 Abs. 2 lit. c).

## 11. Dokumente, die dazugehören

| Dokument | Wo |
|---|---|
| Nutzungsreglement Mail und Internet | [Ablage] |
| Löschkonzept samt Löschliste | [Ablage] |
| Verzeichnis der Bearbeitungstätigkeiten | [Ablage] |
| Verfahrensdokumentation des Archivs | liegt im Archiv selbst, `.filum/verfahren.txt` |
| Einrichtung von Share und Sicherung | [Ablage] |

---

## Für das Büro: was mit diesem Blatt noch zu tun ist

| Schritt | Erledigt am |
|---|---|
| Ablageort, Namen und Fristen eintragen | [ ] |
| Mitarbeiter informieren, zusammen mit dem Nutzungsreglement | [ ] |
| Zugriffsaufzeichnung auf dem NAS einrichten | [ ] |
| Rückspielen der Sicherung einmal testen und das Datum eintragen | [ ] |
| Jährlichen Durchgang im Kalender setzen | [ ] |
