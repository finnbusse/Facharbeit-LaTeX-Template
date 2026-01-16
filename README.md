# Facharbeit LaTeX Template
(Dokumentation mithilfe von KI erstellt)
Dieses Repository enthält ein strukturiertes und modernes LaTeX-Template zur Erstellung von Facharbeiten in der gymnasialen Oberstufe.
Das Template ist darauf ausgelegt, Inhalt, Layout und Metadaten sauber zu trennen und eignet sich besonders für längere wissenschaftspropädeutische Arbeiten.

---

## Ziel des Templates

* Einheitliches, professionelles Layout
* Klare und wartbare Projektstruktur
* Einfache Anpassbarkeit ohne Eingriff in den Haupttext
* Saubere Trennung von

  * Inhalt
  * Design
  * Dokument-Metadaten

---

## Projektstruktur

Facharbeit-LaTeX-Template/
│
├─ main.tex – Zentrale Hauptdatei
│
├─ settings/
│   ├─ metadata.tex – Titel, Autor, Schule, Kurs
│   ├─ preamble.tex – Pakete und Grundeinstellungen
│   ├─ layout.tex – Seitenlayout, Kopf- und Fußzeilen
│   └─ commands.tex – Eigene Befehle und Abkürzungen
│
├─ assets/
│   └─ images/ – Logos und Abbildungen
│
├─ chapters/ – Inhaltliche Kapitel
│
└─ bibliography/
  └─ references.bib – Literaturverzeichnis

---

## Schnellstart

### Projekt herunterladen

* Repository klonen
* oder über **Code → Download ZIP** herunterladen

### Kompilieren

Empfohlene Umgebungen:

* Overleaf
* TeXstudio
* VS Code mit LaTeX Workshop

Kompilationsreihenfolge:
pdflatex → biber → pdflatex → pdflatex

---

## Inhalte anpassen

### Metadaten ändern

Datei: settings/metadata.tex

Beispiel:
\newcommand{\autorname}{Finn Busse}
\newcommand{\arbeitstitel}{Der NEAT-Algorithmus}
\newcommand{\schule}{Christian-Dietrich-Grabbe-Gymnasium}

---

### Kapitel schreiben

Alle Texte liegen im Ordner chapters.
In main.tex werden sie eingebunden:

\input{chapters/einleitung}
\input{chapters/theorie}
\input{chapters/fazit}

---

### Bilder einfügen

Dateien ablegen in: assets/images/

Einbindung im Text:
\includegraphics[width=0.8\textwidth]{assets/images/logo.png}

---

## Literaturverzeichnis

* Quellen werden in bibliography/references.bib gepflegt
* Zitieren im Text:
  \cite{neat2002}

---

## Besonderheiten

* Strikte Trennung von Design und Inhalt
* Geeignet für

  * Facharbeiten
  * Projektarbeiten
  * wissenschaftspropädeutische Arbeiten
* Einfach erweiterbar um

  * Abkürzungsverzeichnis
  * Abbildungsverzeichnis
  * Anhang
  * KI-Nutzungsnachweis

---

## Lizenz und Nutzung

Dieses Template darf frei für schulische und private Zwecke verwendet und angepasst werden.
Bei Weitergabe oder Veröffentlichung bitte einen Hinweis auf dieses Repository beibehalten.

---

## Autor

Finn Busse
Schüler · Informatik · LaTeX

GitHub: [https://github.com/finnbusse](https://github.com/finnbusse)
