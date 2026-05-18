# 📄 Resume Template (LaTeX)

A clean, one-page LaTeX resume template built for software engineers — used by **[Madhav Krishan Goswami](https://github.com/MadhavKrishanGoswami)** and free for anyone to fork and use.

Focused on what recruiters actually read: experience, projects, skills. No icons, no colors fighting for attention, no two-column gimmicks that break ATS parsers.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![LaTeX](https://img.shields.io/badge/LaTeX-resume-008080.svg)
![Pages](https://img.shields.io/badge/length-1%20page-success)

---

## ✨ Features

- **One page, A4** — fits a senior-engineer-density resume without spilling
- **ATS-friendly** — single column, standard fonts, no images
- **Minimal dependencies** — compiles with stock TeX Live / MiKTeX / Overleaf
- **Clean macros** — `\resumeSubheading`, `\resumeItem`, `\resumeProjectHeading` so the source stays readable
- **Hyperlinked header** — email, LinkedIn, GitHub, blog
- **MIT licensed** — fork it, ship it

---

## 📁 Repo Contents

| File | Purpose |
|------|---------|
| `resume.tex` | The blank template with placeholders — start here |
| `example.tex` | A filled-in example (Madhav's actual resume) for reference |
| `LICENSE` | MIT |
| `.gitignore` | Ignores LaTeX build artifacts (`.aux`, `.log`, etc.) |

---

## 🚀 Quick Start

### Option 1: Overleaf (easiest)

1. Click **New Project → Upload Project** on [Overleaf](https://www.overleaf.com).
2. Upload this repo as a `.zip`.
3. Open `resume.tex` and hit **Recompile**.

### Option 2: Local

You need a LaTeX distribution (TeX Live on Linux/Mac, MiKTeX on Windows).

```bash
git clone https://github.com/MadhavKrishanGoswami/resume-template.git
cd resume-template
pdflatex resume.tex
```

The PDF will be generated next to the `.tex` file. Run `pdflatex` twice if cross-references look off.

### Option 3: VS Code

Install the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension, open the folder, and press **Ctrl/Cmd + Alt + B** to build.

---

## ✏️ Customizing

Open `resume.tex` and replace the placeholders:

1. **Header block** — name, phone, email, LinkedIn, GitHub, blog
2. **Experience** — duplicate the `\resumeSubheading { ... }` block per role
3. **Projects** — duplicate `\resumeProjectHeading { ... }` per project
4. **Education** — fill in school, degree, dates, coursework
5. **Skills** — group by category (Languages / Cloud / Backend / Data / Tools)
6. **Certifications & Achievements** — one line each

### Adding a new experience entry

```latex
\resumeSubheading
  {Company Name}{Start -- End}
  {Job Title}{Location}
  \resumeItemListStart
    \resumeItem{Achievement with \textbf{a number} and a clear outcome.}
    \resumeItem{Another bullet — use action verb + tech + measurable result.}
  \resumeItemListEnd
```

### Tips for writing good bullets

- Lead with the result, not the task: *"Reduced API latency by 40%"* beats *"Worked on API performance"*
- Always pair tech with impact: *"Built X in Go, handling Y RPS"*
- Bold the keywords (`\textbf{Go}`, `\textbf{40\%}`) — scanners will catch them
- Keep each bullet to one line if you can; two max

---

## 🖼️ Preview

`example.tex` is Madhav's actual resume — compile it to see what a finished version looks like.

> Add a screenshot here once you fork: `![preview](preview.png)`

---

## 📜 License

[MIT](LICENSE) — free for personal and commercial use. Attribution appreciated but not required.

---

## 🙌 Credits

Created by **Madhav Krishan Goswami**
[GitHub](https://github.com/MadhavKrishanGoswami) · [LinkedIn](https://www.linkedin.com/in/madhavkrishangoswami/) · [Blog](https://madhavkrishangoswami.hashnode.dev/)
