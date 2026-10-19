<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT TITLE BLOCK -->
<br />
<div align="center">
  <a href="https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025">
    <h3 align="center">exam-revision-notes-2025</h3>
  </a>

  <p align="center">
    Study notes, cheat sheets and exam scans for the June 2025 assessment round.<br />
    A notes repository, not an application.
    <br />
    <a href="https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/tree/main/Revisions%20planning"><strong>Start at the index »</strong></a>
    <br />
    <a href="https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/issues">Report Bug</a>
    &middot;
    <a href="https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#what-is-in-this-repository">What is in this repository</a></li>
        <li><a href="#repository-layout">Repository layout</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

This repository is **not a software project**. There is no source code here, no build
system, and nothing to compile or run. It is a personal study vault: notes, cheat
sheets, worked solutions and scanned handouts for the June 2025 exams of a third-year
engineering programme (the notes refer to "3IIR").

It is written as an Obsidian vault. That is visible from two things in the repository:
the `.gitignore` contains a single line, `.obsidian/`, and the notes link to each other
with `[[wikilinks]]` such as `[[Conception]]` and `[[SQLServer]]`. Anything in square
brackets in these notes is a link to another note, not broken markdown.

### What is in this repository

Subject folders, each with its own note style:

| Folder | Contents |
|---|---|
| `Revisions planning/` | The hub. `Index.md` links every date note and every subject sheet. `Planning/` holds one note per exam day (11, 12, 13, 16 and 17 June 2025); four of them just list the exams for that day, and `11-06-2025.md` also carries a short checklist. `Fiches matières/` holds one revision sheet per subject. |
| `Conception/` | Object-oriented modelling with UML. Three notes covering development methods (Y, V, M, spiral, RAD, XP), the exam structure and what to review. |
| `Reseau/` | Networking. Two worked TDs on IP, fragmentation, addressing, subnetting and router routing tables, plus a TCP/IP cheat sheet. |
| `Sql Server/` | T-SQL. A syntax reference and worked walkthroughs of TP3 to TP6 against a `GestionCom` database. |
| `Statistique/` | Statistics. A written summary and a QCM sheet, four PDFs (course support, a TD, the normal-law table, the Student's t table) and ~20 page scans in `pics/`. |
| `Frensh/` | A single PDF, `ALL.pdf`. The folder name is spelled exactly like that in the repository. |

The revision sheets in `Revisions planning/Fiches matières/` are the most useful part
of the repository and follow a consistent shape: an exam breakdown, then a checklist
of what to review, then a progress list with boxes ticked off as work gets done. The
notes mix French and English freely, and `Statistique/Resume.md` also includes Darija
written in Latin script. The intent is working notes for revision, not polished prose.

### Repository layout

```
exam-revision-notes-2025/
├── .gitignore                       # only ".obsidian/"
├── 2, 10, 10 1, 12, 13              # image files with no file extension (see below)
├── Conception/                      # UML and software development methods
├── Frensh/
│   └── ALL.pdf
├── Reseau/                          # TD1, TD3, TCP/IP cheat sheet
├── Revisions planning/
│   ├── Index.md                     # entry point
│   ├── 2025-06-02.md                # empty
│   ├── 2025-06-05.md                # empty
│   ├── Planning/                    # 11-06, 12-06, 13-06, 16-06, 17-06
│   └── Fiches matières/             # 9 subject sheets
├── Sql Server/                      # T-SQL_Syntaxe.md, TP3–TP6
└── Statistique/                     # Resume.md, QCM.md, 4 PDFs, pics/
```

Three rough edges you will notice immediately:

- **Five image files sit at the repository root with no extension** — `2`, `10`,
  `10 1`, `12` and `13`. They are scans and photographs of exam papers that were
  uploaded without a name or a suffix. There is nothing that links to them, and
  `10 1` is a near-duplicate of `10`.
- **`Index.md` links do not resolve as written.** It points at `[[11-06-2025]]` through
  `[[17-06-2025]]`, but those notes live in `Revisions planning/Planning/` while the
  index sits one level up. Obsidian matches links by filename, so they only work if the
  link resolution setting is adjusted or the index is moved into `Planning/`.
- **Two empty notes.** `Revisions planning/2025-06-02.md` and `2025-06-05.md` contain no
  content, and nothing links to them.
- **`Art et culture` is plain text**, not a `[[wikilink]]`, so it is the only subject in
  `Index.md` that is not a link.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

This is a plain-text repository, so "built with" means the file formats it contains.

* [![Markdown][Markdown-badge]][Markdown-url]
* [![Obsidian][Obsidian-badge]][Obsidian-url]
* [![PDF][PDF-badge]][PDF-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* Any text editor or Markdown viewer.
* [Obsidian](https://obsidian.md) if you want the `[[wikilinks]]` to render as links.
  Any editor works otherwise — the notes are plain Markdown.
* A PDF reader for the handouts in `Statistique/` and `Frensh/`.

### Installation

1. Clone the repo

   ```sh
   git clone https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025.git
   cd exam-revision-notes-2025
   ```

2. Open the folder as an Obsidian vault, or just browse the Markdown files in an
   editor. The `.gitignore` already excludes `.obsidian/`, so any local Obsidian
   settings you create will not show up as untracked changes.

3. Start at `Revisions planning/Index.md` for the calendar, or jump straight to the
   `Fiches matières/` sheet for a single subject.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

There is no software to run. The practical way to use this repository is:

- **Plan by day.** Each `Revisions planning/Planning/DD-MM-YYYY.md` note lists the exams
  for that date and a short list of loose ends. `11-06-2025.md`, for example, lists
  `[[Reseau]]` and `[[SQLServer]]` and then `Finir TP SQL`, `Exercices normalisation`
  and `Vérifier contenu Reseau`.
- **Revise by subject.** The `Fiches matières/` sheets carry the exam breakdown and a
  checklist. `Conception.md`, for example, splits the exam into a QCM, a diagram to
  describe or build, and a long exercise on use case, sequence and class diagrams.
- **Work the exercises.** The longer files in `Reseau/` and `Sql Server/` are full
  walkthroughs rather than summaries — `Sql Server/TP3.md` builds a `GestionCom`
  database table by table, and `Reseau/TD3.md` works router exercises question by
  question.
- **Use the tables in `Statistique/`.** `Table Loi Normale.pdf` and
  `Table de Student.pdf` are the lookup tables the `Resume.md` notes refer to when
  reading off critical values.
- **Work through the scans.** `Statistique/pics/` holds the course slides and worked
  examples referenced from `Resume.md` through `![[1.jpg]]`-style embeds.

`Sql Server/T-SQL_Syntaxe.md` is the longest single document in the repository. It
starts from "what is T-SQL?" in plain language and builds up through command
reference tables, joins, subqueries, aggregation and stored procedures.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

Present in the repository today:

- [x] Exam calendar for 11, 12, 13, 16 and 17 June 2025
- [x] Revision sheets for 9 subjects (Reseau, SQLServer, Conception, Francais, Java, Anglais, Statistiques, Art et culture, Programmation lineaire)
- [x] Worked TDs for networking (`TD1`, `TD3`) and a TCP/IP cheat sheet
- [x] T-SQL syntax reference and TP3–TP6 walkthroughs
- [x] Statistics summary, QCM sheet, course PDFs and distribution tables
- [x] UML / development-methods notes for Conception

Known gaps, based on the current state of the files:

- [ ] Fix the `Index.md` wikilinks so they resolve to the notes in `Planning/` and `Fiches matières/`
- [ ] Delete or rename the extensionless image files at the repository root (`2`, `10`, `10 1`, `12`, `13`), or move them into the subject folder they belong to
- [ ] Fill in or remove the empty notes `2025-06-02.md` and `2025-06-05.md` — 2 and 5 June have neither an exam list nor a checklist
- [ ] Turn the `Art et culture` mentions in `Index.md` and `16-06-2025.md` into `[[wikilink]]`s, matching the other eight subjects
- [ ] Renaming `Frensh/` to `French/` — but note that renaming breaks any existing link to the folder
- [ ] Add a `LICENSE` file, since course handouts and third-party PDFs are redistributed here

See the [open issues](https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

Corrections are the most useful contribution here: a wrong critical value in the
Student or normal-law tables, a broken diagram description, or a missing subject on the
calendar. Fork the repo and open a pull request, or open an issue.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Note that the notes use `[[wikilinks]]` between files, so adding a subject sheet means
adding both the file and its `[[link]]` in `Revisions planning/Index.md`.

### Top contributors:

<a href="https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Elouahabi-Naoufal/exam-revision-notes-2025" alt="contrib.rocks image" />
</a>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

No `LICENSE` file is bundled with this repository. That matters more here than in a code
repository: `Statistique/` and `Frensh/` contain course handouts, distribution tables and
photographs that belong to their original authors, not to this repository. The PDFs remain
under their own terms.

This project is not licensed — all rights reserved.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Naoufal Elouahabi - [LinkedIn](https://www.linkedin.com/in/elouahabi-naoufal/) - elouahabi-naoufal1@gmail.com

Project Link: [https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025](https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* The course materials, handouts and exam papers in `Statistique/`, `Frensh/` and `Sql Server/` come from the teaching staff of the programme; this repository only collects and re-types them.
* [Obsidian](https://obsidian.md) for the `[[wikilink]]` format used throughout.
* [Best README Template](https://github.com/othneildrew/Best-README-Template)
* [Img Shields](https://shields.io)
* [contrib.rocks](https://contrib.rocks/)
* [Choose an Open Source License](https://choosealicense.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Elouahabi-Naoufal/exam-revision-notes-2025.svg?style=for-the-badge
[contributors-url]: https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Elouahabi-Naoufal/exam-revision-notes-2025.svg?style=for-the-badge
[forks-url]: https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/network/members
[stars-shield]: https://img.shields.io/github/stars/Elouahabi-Naoufal/exam-revision-notes-2025.svg?style=for-the-badge
[stars-url]: https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/stargazers
[issues-shield]: https://img.shields.io/github/issues/Elouahabi-Naoufal/exam-revision-notes-2025.svg?style=for-the-badge
[issues-url]: https://github.com/Elouahabi-Naoufal/exam-revision-notes-2025/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/elouahabi-naoufal/
[Markdown-badge]: https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white
[Markdown-url]: https://daringfireball.net/projects/markdown/
[Obsidian-badge]: https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white
[Obsidian-url]: https://obsidian.md/
[PDF-badge]: https://img.shields.io/badge/PDF-B30E0E?style=for-the-badge&logo=adobepdf&logoColor=white
[PDF-url]: https://www.adobe.com/acrobat/about-adobe-pdf.html