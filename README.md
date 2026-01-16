<div align="center">

# 📚 Facharbeit LaTeX Template

### Professionelles LaTeX-Template für wissenschaftspropädeutische Arbeiten

[![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)](https://www.latex-project.org/)
[![License](https://img.shields.io/badge/Lizenz-Frei_für_Schulen-blue?style=for-the-badge)](LICENSE)
[![Made with Love](https://img.shields.io/badge/Made_with-❤️-red?style=for-the-badge)](https://github.com/finnbusse)

*Dokumentation mithilfe von KI erstellt*

[Features](#-features) • [Schnellstart](#-schnellstart) • [Projektstruktur](#-projektstruktur) • [Anpassung](#-inhalte-anpassen) • [Dokumentation](#-literaturverzeichnis)

</div>

---

## 🎯 Über das Template

Dieses Repository enthält ein **strukturiertes und modernes LaTeX-Template** zur Erstellung von Facharbeiten in der gymnasialen Oberstufe. Das Template ist darauf ausgelegt, Inhalt, Layout und Metadaten sauber zu trennen und eignet sich besonders für längere wissenschaftspropädeutische Arbeiten.

## ✨ Features

<table>
<tr>
<td width="50%">

### 🎨 **Design & Layout**
- ✅ Einheitliches, professionelles Layout
- ✅ Moderne Seitengestaltung
- ✅ Anpassbare Kopf- und Fußzeilen
- ✅ Professionelle Titelseite

</td>
<td width="50%">

### 🔧 **Struktur & Organisation**
- ✅ Klare und wartbare Projektstruktur
- ✅ Strikte Trennung von Inhalt & Design
- ✅ Modularer Aufbau
- ✅ Einfache Anpassbarkeit

</td>
</tr>
<tr>
<td width="50%">

### 📖 **Funktionalität**
- ✅ Automatisches Literaturverzeichnis
- ✅ Abbildungs- und Tabellenverzeichnis
- ✅ Anhang-Verwaltung
- ✅ KI-Nutzungsnachweis

</td>
<td width="50%">

### 🚀 **Verwendung**
- ✅ Facharbeiten
- ✅ Projektarbeiten
- ✅ Wissenschaftspropädeutische Arbeiten
- ✅ Seminararbeiten

</td>
</tr>
</table>

---

## 📁 Projektstruktur

```
Facharbeit-LaTeX-Template/
│
├── 📄 main.tex                    # Zentrale Hauptdatei
│
├── ⚙️  settings/                   # Konfiguration & Einstellungen
│   ├── metadata.tex               # Titel, Autor, Schule, Kurs
│   ├── preamble.tex               # Pakete und Grundeinstellungen
│   ├── layout.tex                 # Seitenlayout, Kopf- und Fußzeilen
│   └── commands.tex               # Eigene Befehle und Abkürzungen
│
├── 🎨 assets/                      # Ressourcen
│   ├── images/                    # Logos und Abbildungen
│   └── tables/                    # Externe Tabellen
│
├── 📝 content/                     # Inhaltliche Kapitel und Dokumente
│   ├── 01_einleitung.tex
│   ├── 99_copyright.tex
│   └── ...
│
├── 📚 bib/                         # Literaturverwaltung
│   ├── literature.bib             # Bücher und Artikel
│   ├── internet.bib               # Internetquellen
│   └── gen-ai.bib                 # KI-Quellen
│
└── 📎 appendix/                    # Anhang
    └── 01_code.tex
```

---

## 🚀 Schnellstart

### 1️⃣ Projekt herunterladen

**Option A: Git Clone**
```bash
git clone https://github.com/finnbusse/Facharbeit-LaTeX-Template.git
cd Facharbeit-LaTeX-Template
```

**Option B: ZIP-Download**
- Klicke auf **Code → Download ZIP**
- Entpacke das Archiv

### 2️⃣ Kompilieren

#### Empfohlene Umgebungen:

| Tool | Beschreibung |
|------|-------------|
| 🌐 **[Overleaf](https://www.overleaf.com/)** | Online LaTeX-Editor (empfohlen für Einsteiger) |
| 💻 **[TeXstudio](https://www.texstudio.org/)** | Desktop-Editor mit integrierter Vorschau |
| 🆚 **[VS Code](https://code.visualstudio.com/)** | Mit LaTeX Workshop Extension |

#### Kompilationsreihenfolge:
```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

> **💡 Tipp:** In den meisten LaTeX-Editoren genügt ein Klick auf „Kompilieren", die Reihenfolge wird automatisch ausgeführt.

---

## 🛠️ Inhalte anpassen

### 📋 Metadaten ändern

Öffne `settings/metadata.tex` und passe die Angaben an:

```latex
\newcommand{\autorname}{Dein Name}
\newcommand{\arbeitstitel}{Dein Arbeitstitel}
\newcommand{\schule}{Deine Schule}
\newcommand{\kurs}{Dein Kurs}
\newcommand{\fach}{Dein Fach}
\newcommand{\abgabedatum}{TT.MM.JJJJ}
```

### ✍️ Kapitel schreiben

1. Erstelle oder bearbeite Dateien im Ordner `content/`
2. Binde sie in `main.tex` ein:

```latex
\input{content/01_einleitung}
\input{content/02_hauptteil}
\input{content/03_fazit}
```

### 🖼️ Bilder einfügen

1. Lege Bilder in `assets/images/` ab
2. Binde sie im Text ein:

```latex
\begin{figure}[h]
  \centering
  \includegraphics[width=0.8\textwidth]{assets/images/mein-bild.png}
  \caption{Beschreibung des Bildes}
  \label{fig:mein-bild}
\end{figure}
```

### 📚 Literatur zitieren

1. Füge Quellen in `bib/literature.bib` hinzu:

```bibtex
@book{mustermann2023,
  author = {Max Mustermann},
  title = {Ein tolles Buch},
  year = {2023},
  publisher = {Beispielverlag}
}
```

2. Zitiere im Text:

```latex
\cite{mustermann2023}
```

---

## 🎓 Erweiterte Features

Das Template kann einfach um folgende Elemente erweitert werden:

- 📑 **Abkürzungsverzeichnis** – Liste verwendeter Abkürzungen
- 🖼️ **Abbildungsverzeichnis** – Automatische Auflistung aller Abbildungen
- 📊 **Tabellenverzeichnis** – Übersicht aller Tabellen
- 📎 **Anhang** – Für zusätzliche Materialien
- 🤖 **KI-Nutzungsnachweis** – Dokumentation von KI-Unterstützung

---

## 📄 Lizenz und Nutzung

Dieses Template darf **frei für schulische und private Zwecke** verwendet und angepasst werden. Bei Weitergabe oder Veröffentlichung bitte einen Hinweis auf dieses Repository beibehalten.

> **Lizenz:** Frei verwendbar mit Quellenangabe (MIT-ähnlich)

---

## 👨‍💻 Autor

<div align="center">

**Finn Busse**

*Schüler · Informatik · LaTeX*

[![GitHub](https://img.shields.io/badge/GitHub-finnbusse-181717?style=for-the-badge&logo=github)](https://github.com/finnbusse)

</div>

---

<div align="center">

### ⭐ Gefällt dir das Template?

Gib dem Projekt einen **Stern** auf GitHub!

**Viel Erfolg bei deiner Facharbeit!** 🎓

</div>
