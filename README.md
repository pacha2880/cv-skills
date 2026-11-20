# cv-skills

An agent skill for Claude Code that writes one-page, Harvard-style CVs in LaTeX and hands you a PDF
ready to send.

The skill works like a careful reviewer, not a form filler:

1. **Interviews you first**: what the CV is for, which roles, language, country, how many versions.
2. **Waits for your material**: old CV, LinkedIn, GitHub, job postings, certificates.
3. **Asks about gaps and contradictions** (dates, titles, missing numbers) instead of guessing.
4. **Critiques honestly** before rewriting, and never invents facts.
5. **Writes, compiles and checks** the CV: one page, one line per bullet, reverse chronological order.

It can also prepare how to explain a short job or a firing in an interview.

## What's inside

```
cv-writer/
  SKILL.md                    the workflow the agent follows
  references/writing-guide.md the rules: format, bullets, tailoring, honesty, Spanish CVs
  template/harvardcv.sty      the LaTeX layout
  template/example-cv.tex     an example CV for a fictional person
  template/example-cv.pdf     the compiled example
```

See [the example PDF](cv-writer/template/example-cv.pdf).

## Install

Copy the `cv-writer` folder into your skills directory:

```bash
git clone https://github.com/pacha2880/cv-skills.git
cp -r cv-skills/cv-writer ~/.claude/skills/
```

Then ask Claude Code something like "help me rebuild my CV for backend roles".

## Requirements

- XeLaTeX (TeX Live or MiKTeX). The font, TeX Gyre Termes, ships with both. No local TeX? Upload the
  folder to Overleaf and set the compiler to XeLaTeX.
- Optional: poppler (`pdfinfo`, `pdftotext`, `pdftoppm`) so the agent can check page count and line wraps.

## Use the template without the skill

```bash
cd cv-skills/cv-writer/template
xelatex example-cv.tex
```

Edit `example-cv.tex`. The macros are `\header`, `\role`, `\shortrole` and `\school`, described at the
top of `harvardcv.sty`.

## License

MIT
