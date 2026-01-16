```md
# Facharbeit LaTeX Template
(Dokumentation mithilfe von KI erstellt)
Dieses Repository enthält ein strukturiertes und modernes LaTeX-Template zur Erstellung von Facharbeiten in der gymnasialen Oberstufe.  
Das Template ist darauf ausgelegt, eine saubere Trennung von Inhalt, Layout und Metadaten zu ermöglichen und eignet sich besonders für längere wissenschaftspropädeutische Arbeiten.

---

## 🎯 Ziel des Templates

- Einheitliches, professionelles Layout  
- Klare Projektstruktur  
- Einfache Anpassbarkeit ohne Eingriff in den Haupttext  
- Saubere Trennung von:
  - Inhalt  
  - Design  
  - Dokument-Metadaten  

---

## 📁 Projektstruktur

```

Facharbeit-LaTeX-Template/
│
├─ main.tex                → Hauptdatei
│
├─ settings/
│   ├─ metadata.tex        → Titel, Autor, Schule, Kurs etc.
│   ├─ preamble.tex        → Pakete & Grundeinstellungen
│   ├─ layout.tex          → Seitenlayout, Kopf-/Fußzeilen
│   └─ commands.tex        → Eigene Befehle & Abkürzungen
│
├─ assets/
│   └─ images/             → Logos & Abbildungen
│
├─ chapters/               → Inhaltliche Kapitel
│
└─ bibliography/
└─ references.bib      → Literaturverzeichnis

```

---

## 🚀 Schnellstart

### 1. Projekt herunterladen
- Repository klonen  
- oder **Code → Download ZIP**

### 2. Kompilieren
Empfohlene Umgebungen:
- **Overleaf**
- **TeXstudio**
- **VS Code + LaTeX Workshop**

Kompilationsreihenfolge:
```

pdflatex → biber → pdflatex → pdflatex

````

---

## ✏️ Inhalte anpassen

### Metadaten ändern  
Datei: `settings/metadata.tex`

Beispiel:
```latex
\newcommand{\autorname}{Finn Busse}
\newcommand{\arbeitstitel}{Der NEAT-Algorithmus}
\newcommand{\schule}{Christian-Dietrich-Grabbe-Gymnasium}
````

---

### Kapitel schreiben

Alle Texte liegen im Ordner `chapters/`.
In `main.tex` werden sie eingebunden:

```latex
\input{chapters/einleitung}
\input{chapters/theorie}
\input{chapters/fazit}
```

---

### Bilder einfügen

Dateien ablegen in:

```
assets/images/
```

Einbindung im Text:

```latex
\includegraphics[width=0.8\textwidth]{assets/images/logo.png}
```

---

## 📚 Literaturverzeichnis

* Quellen in `bibliography/references.bib` pflegen
* Zitieren im Text:

```latex
\cite{neat2002}
```

---

## 🧩 Besonderheiten

* Klare Trennung von Design und Inhalt
* Geeignet für:

  * Facharbeiten
  * Projektarbeiten
  * wissenschaftspropädeutische Arbeiten
* Einfach erweiterbar um:

  * Abkürzungsverzeichnis
  * Abbildungsverzeichnis
  * Anhang
  * KI-Nutzungsnachweis

---

## 📜 Lizenz & Nutzung

Dieses Template darf frei für schulische und private Zwecke verwendet und angepasst werden.
Bei Weitergabe oder Veröffentlichung bitte einen Hinweis auf dieses Repository beibehalten.

---

## 👤 Autor

**Finn Busse**
Schüler · Informatik · LaTeX

GitHub: [https://github.com/finnbusse](https://github.com/finnbusse)

```
```
