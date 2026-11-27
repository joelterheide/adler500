# Adler 500 – Schreibmaschine für Essays

Eine ablenkungsfreie Schreibmaschine im Browser: eine Zeile unter der Lampe, Tastenklang, Glocke, Wagenrücklauf – und ein Archiv mit animiertem Schreibprotokoll.

## Funktionen
- **Schreibmaschinen-Gefühl:** Lampe und Typenhebel bleiben mittig, das Blatt läuft beim Tippen durch (umstellbar auf „Kopf wandert“). Das Blatt wird zeilenweise hochgezogen, der Wagen springt zurück, die Glocke klingelt beim Zeilenumbruch.
- **Nur vorwärts (⌫-Knopf):** Löschen, Rückgängig und Cursor-zurück sind gesperrt.
- **Archiv / Logbuch:** Jeder Text wird automatisch gespeichert. Mit ✓ abschließen → Schreibprotokoll (Wörter, Schreibzeit, Anschläge, Tempo, Seiten, Sitzungen) mit animierter Route zum Wortziel. Im Archiv: Gesamtstatistik, Wörter pro Tag (14 Tage), Serie, Suche, Wieder öffnen, Lesen, Export, Löschen.
- **Einstellungen:** Papier, Schrift (8 Schreibmaschinenschriften), Maschine (Klang), Schriftgröße, Zeilenbreite · Lampe (Wärme, Helligkeit, Lichtkegel) · Ton (Tasten, Glocke, Wagen, Atmosphäre: Wald, Sommernacht, Strand, Regen, Kamin) · Wortziel, Wortumbruch.
- **Export:** PDF, Word (.docx), .txt, .md, Zwischenablage, Teilen – auf iPhone/iPad über das Teilen-Menü („In Dateien sichern“). Archiv-Sicherung als JSON (und wieder einlesen).
- **Offline & als App:** Funktioniert offline (Service Worker) und lässt sich auf dem iPhone über „Zum Home-Bildschirm“ installieren.

## Bedienung
- **Nach unten wischen:** Lampe, Leisten und Wagen blenden aus – nur noch die Schrift. Dort scrollt man mit einem Finger durch den ganzen Text; unten angekommen holt nach oben wischen alles zurück (Desktop: `⌘/Strg + .` bzw. `Esc`).
- Zurückblättern: Mausrad, Pfeiltasten oder mit zwei Fingern wischen.
- `⌘/Strg + S` speichern · `⌘/Strg + Enter` abschließen · `Esc` schließt Fenster.

## Starten
Einfach `index.html` im Browser öffnen – oder über GitHub Pages hosten (Settings → Pages → Branch wählen).
Für Service Worker/Installation muss die Seite über `http(s)` laufen, z. B. lokal: `python3 -m http.server`.

Alle Texte liegen nur lokal im Browser (localStorage). Sichere dein Archiv regelmäßig über „Archiv sichern“.

## Klänge
Tastenanschläge und Glocke stammen aus der Aufnahme „Typewriter typing“ (freesound_community, über Pixabay), in `sounds/typewriter.wav` als einzelne Ausschnitte zusammengefasst. Atmosphären „Vögel auf dem Land“ (strachszydlo), „Regen“ (universfield) und „Meereswellen“ sind gekürzte, lautstärkeangeglichene Ausschnitte aus vom Nutzer bereitgestellten Aufnahmen (`sounds/*.m4a`). Wagenrücklauf und die mit „synth.“ markierten Atmosphären werden im Browser erzeugt.
