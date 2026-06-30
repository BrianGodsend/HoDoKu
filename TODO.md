# TODO

## High Priority

## Backlog

- [ ] user created arrows (3022071)
- [ ] Add a pattern generator to sudoku creation that allows a user to specify which cells should contain givens.
      (2940097) - doesnt work correctly: no valid puzzles are found
- [ ] Add animation for automatic solving (3387362)

## Completed

### Most Recent

- [x] Alt-click for candidates (3387344)
- [x] Undo leads to incorrect hints (3260556) (2963769)
- [x] Hints when "Show all candidates" is not selected (3387347)
- [x] Add mouse click detection (3387327)
- [x] Tooltips for alle Knopfe und Menus (2990569)
- [x] Add extended print options (3387351)
- [x] Add progress and success marker (3387345)
- [x] create puzzles in the background (3011686) (2940101)
- [x] Store difficulty level between runs (3394539)
- [x] fix "Print solution" (3387212)
- [x] highlight more than one candidate (3324082)
      `<ctrl>-<click>` um mehrere Kandidaten auszuwohlen
      ????? wenn alle Kandidate in der Zelle sind oder wenn irgendein Kandidat in der Zelle ist ???????
- [x] Nimbus: selected techniques are not highlighted (3303097)
- [x] It should be possible to remove candidates from a group of cells via the keyboard. If the candidate is set
     in at least one cell, the candidate is removed from all cells else it is set in all cells. (3296914)
- [x] The following grid causes a "Multiple Solutions" warning in version 2.0.1. (see sf.net) (3214361)
- [x] rework loading of incorrect puzzles (3144406) (2970905)
- [x] Hidden Pair incorrectly identified as Locked Pair (3134693)
- [x] Create Sudoku Window hangs (3098767)
- [x] The 'Show Deviations' option is not being remembered every time a new game is started. The option to show
     deviations on startup is unchecked in the options, and it is off when starting HoDoKU up, but it
     automatically turns itself back on every time the new game button is clicked. (3054092)
- [x] puzzle creation training mode: accept any puzzle that contains one of the training techniques (2995579)
- [x] Arrows drawn incorrectly (2954459)
- [x] Load hodoku.hcfg from program directory (2940096)
- [x] UR with missing candidates (2689169)
- [x] Hide hint pane, toolbar; fullscreen? (3387335)
- [x] Change display of focus (3387341)
- [x] Set value in group of cells is broken (3387353)
- [x] Add filter for bivalue cells (3387355)
- [x] Add mode as startup options (3387356)
- [x] Add "vage hint" and "concrete hint" buttons in the hint pane (3387357)
- [x] Add "solve up to" feature (3387359)
- [x] Rework display position of fonts; (make size in cell view configurable - not now)
- [x] gesetzt Zellen nicht forben (konfigurierbar) (3394519)

### Older

- [x] Bugs in Grouped Continuous Nice Loop fixen (Group nodes und ALS fehlerhaft)
- [x] Bug in Forcing Net: "700000004020600010005000800030910000000050000000203090800000700060009020004000005"
   :0000:x:7.......4.2.6...1.+6.5.+9.8.+2.3.91.......+45+6+2.....2.3.9.8.....7...6...9.2...4.....5:112 813 815 318 748 848 152 162 762 862 163 667 169 972 378 179 181 184 384 192 795 895 796 896 698::
   Alles ab 1. ALS loschen -> Alle Schritte -> Forcing Nets gibt Exception
   Probleme bei obervollen TableEntries
- [x] Bug in XY-Chain: Shorter chain available: r1c1 -9- r3c2 -2- r3c6 -7- r3c4 => r1c45,r3c1<>6
   :0702:6:.84..53.7..1493.....3.8..412.73.61..3.8...4..1.98....3.1..7.23...2.3....83.2..71.:522 622 731 931 532 632 732 548 549 255 958 959 571 671 581 681 981 482 582 682 984 986 988 989:614 615 631:
   XY-Chain: 6 r1c1 -9- r7c1 -4- r8c1 -7- r8c2 -9- r3c2 -2- r3c6 -7- r3c4 => r1c45,r3c1<>6
- [x] Bug bei BUG+1: Wenn der 3x vorhandene Kandidat nicht in der Zelle mit den 3 Kandidaten liegt, ist es
   kein BUG+1. Auoerdem werden zu viele Kandidaten geloscht.
   :0610::+5+4..9.8.1392..8.+5..+1.....2..3+46..5+926+2..4.+1.31+59..3.4..8+5.....+7.+7+18+3.4654+63.5.+2..:714 716 724 625 733 434 734 636 736 637 737 639 745 754 756 765 174 274 175 276 976 994 196:176 276 476 676:
- [x] Bei paste: nach Losung wird noch einmal gelost...
- [x] AIC einfohren (gepaart mit Nice Loops)
- [x] Coloring (GUI, Simple, Multiple, Medusa) - Medusa fehlt!
- [x] CopyPaste von SimpleSudoku
- [x] Goltigkeit des Sudokus beim Einfogen profen
- [x] Chaining: Jeweils Chains mit und ohne ALS erstellen (gibt unterschiedliche Eliminierungen bei Nice Loops/AICs)
- [x] Anzeige Forcing Chains/Nets: Einzelne Chains auswohlen und anzeigen
- [x] BUG: Can't copy paste from the Hinweise-Textbox anymore
- [x] BUG:
   :1101:1456:.23759..687.26.59.9.....72.....4.97.3.7.96..2....27...5..47.........2....8...5...:132 432 133 433 839 141 349 661 662 663 364 167 467 867 168 468 568 868 369 379 181 481 184 384 884 389 191 491 194 394 399:143 163 463 672 682:
   Sue de coq (das korzere): 5 ist nicht eliminiert von r6c2!
- [x] BUG:
   :1101:24567:......695.3.5..4.85...4.3.7..63...4.154276839.23..47......9....2.5..897.391....8.:921 168 674 774 776 178 278:299 685:
   Eliminierungen for 1 fehlen in r7c6 und r8c5
- [x] Mehrere Losungen zulassen (inkl. speichern)
- [x] Konfigurationsdialoge oberarbeiten (Farben for Coloring?)
      - BUG: Bei Continuous Nice Lops und AICs Chaindarstellung erweitern
- [x] Hilfe Meno mit About (License)
- [x] Englische version
- [x] EXE-stub (Launch4j)
- [x] User Manual
- [x] Regression tests + Library oberarbeiten
- [x] Doubly linked ALS-xz [http://www.sudoku.com/boards/viewtopic.php?t=3979&postdays=0&postorder=asc&start=0](http://www.sudoku.com/boards/viewtopic.php?t=3979&postdays=0&postorder=asc&start=0)

## 2010-01-17

- [x] Old todo
      - hodoku.hcfg aus Startverzeichnis laden, wenn es existiert.
      - Pattern-Generator: Zellen angeben, die Givens enthalten sollen
      - Hintergrund-Bild erlauben
- [x] ShortCut der zur nochsten erlaubten Zelle springt, wenn Filter gesetzt sind
- [x] Einzelne Kandidaten forben
- [x] Optionen Speichern beim Beenden des Dialogs
      - Add tooltip texts
- [x] Learning Mode: Play, Learn, Practise
      Technik(en) aussuchen, Puzzle wird bei "Learn" bis zur Technik gelost, bei "Practise" wird nur ein
      entsprechendes Puzzle erzeugt
      - generate game in idle time
- [x] Maussteuerung:
      - Double click on a single should set the cell (HS only when filters are applied)
      - Double click on a candidate should set the cell to that value
      - Ctrl-Click on a candidate location should toggle that candidate
      - Double click on a NS should change filter to that digit (?)
      - Right click gibt Kontextmeno mit bester Option zuerst
      - Coloring Zellen: Farbe wohlen, Klick/Shift Klick toggelt
      - Coloring Kandidaten: Wie oben
- [x] Savepoints setzen
      - Automatisches Entfernen von Kandidaten abwohlbar machen
- [x] History of generated puzzles
      - Automatic error report when invalid candidate eliminations are done by the program
      - DUAL Skyscrapers
- [x] URs with missing candidates
- [x] Backdoor searcher (configurable)
- [x] Add "advancing rating" to steps (configurable)
- [x] Allow different sorting options in "show all steps"
      - Add Grouped W-Wing
- [x] BUG: CNL that force candidates
- [x] BUG: Importing invalid puzzles doesnt reset views
- [x] BUG: Copying invalid grids to the clipboard is broken
- [x] BUG: Shortest XY-Chain not found
- [x] BUG: Ist "Alle Kandidaten anzeigen" nicht gesetzt, funktioniert der Gronfilter nicht
- [x] BUG: Shortcuts for difficulty levels dont work correctly
