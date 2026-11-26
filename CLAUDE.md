# Projektregeln: Mathe-Applets

Diese Regeln gelten für jede Sitzung in diesem Repository.

## Zweck

Eine wachsende **Sammlung einzelner Mathe-Applets** für den Unterricht in der gymnasialen Oberstufe (Baden-Württemberg, Berufliches Gymnasium). Jedes Applet ist ein Werkzeug für eine bestimmte Stunde. Die Sammlung ist **keine** zusammenhängende Lernumgebung und kein Kurs. Die Mathe-Lernumgebung ist ein eigenes, getrenntes Repository.

- Die Lernenden bekommen immer nur den Link oder QR-Code zu **einem einzelnen Applet**.
- Applets sind nach **Themen** gruppiert.
- Neue Applets werden erst gebaut, wenn die Lehrkraft eines beschreibt. Keine Beispiel- oder Platzhalter-Applets auf Vorrat.

## Zusammenarbeit

- Die Lehrkraft hat keine Programmierkenntnisse. Technische Arbeiten übernimmt Claude und erklärt Entscheidungen verständlich.
- Sprache im Chat: Deutsch, Anrede „du“, sachlich.
- Anrede in den Applets: „Sie“, außer die Lehrkraft wünscht etwas anderes.
- Rückfragen nur, wenn wesentliche Angaben fehlen. Kleine Gestaltungsfragen selbst entscheiden.
- Unterlagen (Arbeitsblätter, Lösungen, Bildungsplan) hängt die Lehrkraft im Chat an. Ordner auf ihrem Rechner sind nicht sichtbar. Anhänge aus früheren Sitzungen sind nicht mehr vorhanden.
- Nichts als erledigt melden, was nicht geprüft wurde.

## Aufbau

    CLAUDE.md                      diese Regeln
    README.md                      Übersicht aller Applets für die Lehrkraft, nach Themen gruppiert
    index.html                     neutrale Startseite ohne Liste und ohne Links
    <thema>/<applet>/index.html    ein Applet je Ordner

- Themenordner, zum Beispiel `stochastik`, `funktionen`, `differentialrechnung`, `integralrechnung`, `vektorgeometrie`, `matrizen`. Ein Themenordner entsteht erst mit seinem ersten Applet.
- Passt ein Applet zu keinem vorhandenen Thema oder zu mehreren, wird nachgefragt.
- Ordnernamen: Kleinbuchstaben, Bindestriche, keine Umlaute und keine Leerzeichen.
- **Veröffentlichte Ordner nie umbenennen, verschieben oder löschen**, sonst funktionieren Links und QR-Codes nicht mehr. Ausnahme nur auf ausdrücklichen Wunsch, mit Hinweis auf diese Folge.
- In `README.md` steht je Applet: Titel, ein Satz zum Einsatz und der vollständige Link, gruppiert unter einer Überschrift je Thema.

## Technik

- Jedes Applet ist **eine einzige, eigenständige HTML-Datei** (HTML, CSS und JavaScript darin). Kein Build, keine Installation.
- Nichts von fremden Servern laden (keine CDNs, Schriften, Tracker). Ist eine Ausnahme fachlich nötig (zum Beispiel GeoGebra), vorher fragen und den Datenschutz nennen.
- Nichts speichern und nichts übertragen. Keine Eingabe von Namen oder anderen persönlichen Daten.
- Jede Seite enthält `<meta name="robots" content="noindex, nofollow">` und die Viewport-Angabe für Handys.
- Applets verlinken **nicht** auf andere Applets, die Startseite oder das Repository.
- Änderungen an einem Applet verändern keine anderen Applets. Kein gemeinsamer Code zwischen Applets.

## Didaktik und Gestaltung

- Ein Applet hat ein klares Lernziel und enthält nichts Unnötiges.
- Fachsprache, Bezeichnungen und Farben wie auf den Unterlagen der Lehrkraft.
- Lösungen werden nicht vorweggenommen: Farben, Reihenfolge oder Beschriftungen dürfen die richtige Antwort nicht verraten.
- Rückmeldungen geben bei Fehlern einen hilfreichen Hinweis, ohne die Lösung zu nennen.
- Zuerst für das Handy gestalten, mit Finger und Tastatur bedienbar, gut lesbare Kontraste. Information nicht nur über Farbe vermitteln.
- Fehler oder Unstimmigkeiten in den Unterlagen werden der Lehrkraft gemeldet und im Applet korrekt umgesetzt, nicht stillschweigend übernommen.

## Prüfung vor der Vorschau

- Alle Lösungen unabhängig nachrechnen.
- Im Browser testen: richtige und falsche Eingaben, Neustart, keine Konsolenfehler.
- Breiten 320, 390, 768 und 1100 px ohne waagerechtes Scrollen.
- Nennen, was nicht geprüft werden konnte.

## Ablauf: Entwurf, Freigabe, Veröffentlichung

GitHub Pages veröffentlicht den Branch `main` (Ordner `/ (root)`). **Alles auf `main` wird öffentlich.**

1. Kurz zusammenfassen, was gebaut wird, wenn die Beschreibung Spielraum lässt.
2. Auf einem Branch `entwurf/<applet>` bauen und prüfen. Den Entwurfsbranch committen und pushen ist erlaubt.
3. Der Lehrkraft die HTML-Datei zum Ausprobieren schicken.
4. **Nur nach ausdrücklicher Freigabe** im Chat (zum Beispiel „Du kannst es veröffentlichen“) nach `main` übernehmen. „Passt“ oder „ok“ allein genügt nicht, dann nachfragen. Veröffentlicht wird die Fassung, die die Lehrkraft gesehen hat.
5. Mit dem Applet zusammen die Übersicht in `README.md` ergänzen.
6. Den Veröffentlichungslauf prüfen, soweit das möglich ist. Ist die Live-Seite nicht abrufbar, das sagen und die Lehrkraft bitten, den Link selbst zu testen.
7. Den Link nennen und einen QR-Code als Bild schicken. Den QR-Code vorher maschinell auslesen und mit dem Link vergleichen. QR-Bilder kommen nicht ins Repository.

Reine Änderungen an `CLAUDE.md` dürfen auf Wunsch der Lehrkraft direkt nach `main`.

## Links

    https://<github-name>.github.io/<repository>/<thema>/<applet>/

## Datenschutz und Urheberrecht

- Das Repository ist **öffentlich**, auch alle Branches. Nichts Vertrauliches committen.
- Keine Arbeitsblätter, Lösungsblätter, Abbildungen daraus, Verlagsmaterialien oder Original-Prüfungsaufgaben ins Repository. Sie dienen nur als Vorlage, Texte und Aufgaben werden eigenständig formuliert.
- Keine Namen von Schülerinnen, Schülern, Klassen oder der Schule und keine Schülerdaten.
- Getrennte Links sind **kein Zugriffsschutz**. Wer die Adresse kennt, kann jedes Applet öffnen.
