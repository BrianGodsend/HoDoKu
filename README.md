# Hodoku2

An updated version of HoDoKu — a Sudoku generator, solver, analyzer, and trainer written in Java/Swing.

This is a fork of [Hodoku2](https://github.com/wyzelli/Hodoku2) by [wyzelli](https://github.com/wyzelli), which is a fork of [Hodoku](https://github.com/PseudoFish/Hodoku) by [PseudoFish](https://github.com/PseudoFish), which is a fork of [hodoku](https://github.com/yoki123/hodoku) by [yoki123](https://github.com/yoki123), which is a clone of [HoDoKu](https://hodoku.sourceforge.net/en/index.php) originally created by Bernhard Hobiger (hobiwan), who has since passed away.

## Features

- Completely scalable, self-explanatory user interface
- Create random puzzles in five configurable difficulty levels
- Supports over 70 human-style solving techniques (singles, subsets, fish, wings, chains, ALS, and more)
- English and German localization
- Fully configurable via a comprehensive preferences dialog
- Powerful booklet printer and extended print options
- Learning and training modes

## Running

**Windows** — run the provided `HoDoKu.exe` (requires Java 11+ on your PATH).

**All platforms** — run the JAR directly:

```bash
java -Xmx256m -jar hodoku-2.3.2.jar
```

## Building

**Prerequisites:** Java 11+ JDK, Maven 3.8+.

### Executable JAR + Windows EXE

```bash
mvn package
```

Outputs:

| File                        | Description                                                  |
|-----------------------------|--------------------------------------------------------------|
| `target/hodoku-2.3.2.jar`   | Runnable JAR — `java -jar` on any platform                   |
| `target/HoDoKu.exe`         | Windows launcher (Launch4J wrapper; requires Java on PATH)   |

### Windows installer (bundles JRE — no Java required on target machine)

```bash
mvn package -Pinstaller
```

Output: `target/installer/HoDoKu-2.3.2.exe`

**Windows prerequisites for the installer** (one of):

- [Inno Setup 6](https://jrsoftware.org/isinfo.php) — for JDK 18+ builds (recommended)
- [WiX Toolset 3](https://wixtoolset.org/) — for JDK 14–17 builds

### All three artifacts at once

```bash
mvn package -Pinstaller
```

The `package` phase always produces the JAR and EXE. Adding `-Pinstaller` continues through the `verify` phase to also produce the installer.

## Project structure

```text
src/
  main/
    java/
      generator/   # Puzzle generation
      solver/      # All solving techniques
      sudoku/      # UI, main entry point (sudoku.Main), core data model
    resources/
      help/        # HTML keyboard reference (EN + DE)
      img/         # Icons and images
      intl/        # Localization .properties files (EN + DE)
      templates.dat
forms/             # NetBeans GUI Builder .form files (IDE reference only)
exemplars-1.0.txt  # Example puzzles data
reglib-1.3.txt     # Regression library
templates.dat      # Runtime template data
CHANGELOG.md
```

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for the full version history.
