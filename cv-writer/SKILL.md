---
name: cv-writer
description: Write or rebuild a one-page Harvard-style CV (resume) in LaTeX and deliver a ready PDF. Interviews the person first (target role, language, country, number of versions), waits for their material (old CV, LinkedIn, GitHub, job postings, certificates), critiques it honestly, then writes, compiles and checks the CV. Use when someone asks to write, fix, shorten, tailor, translate or review a CV or resume, or to prepare how to explain a gap or a job that ended badly.
---

# CV writer

Build a CV the person can send today: one page, Harvard format, every line true, written the way they
would say it. The template is in `template/` (`harvardcv.sty` for the layout, `example-cv.tex` as the
model to copy). The writing rules are in `references/writing-guide.md`: read it before the first draft.

## 1. Interview first

Ask before writing anything, a few questions at a time, in the person's language:

1. What is the CV for? The role, the industry, a specific job posting (ask for the link or text).
2. How many versions? One per target role is normal (e.g. customer service, engineering, management),
   sharing the same facts with different emphasis.
3. Language of the CV, and the country it is for (Letter paper for the US and Canada, A4 elsewhere).
4. Page limit. Default one page; two only for long senior careers or academic CVs.
5. What makes them stand out (an award, a rare skill, a big name employer)? It should be visible at a
   glance but not take most of the page.

## 2. Collect material, then wait

Ask for everything they have, and say you will wait until they say they are done:

- Current CV in any format (PDF, Word, LaTeX, pasted text) and older versions.
- LinkedIn URL. LinkedIn blocks automated reads behind a sign-in wall: if you have a browser the person
  is signed in to, use it; otherwise ask them to paste the profile or export it as PDF.
- GitHub, portfolio, personal site, competition profiles (read public pages yourself).
- The job postings they are aiming at.
- Certificates, course lists, thesis title, test scores (e.g. language level).

Do not start writing while they are still sending files.

## 3. Build a fact sheet and ask about the gaps

Put every job, project, degree and certificate in one list with dates. Then ask, in one batch:

- Contradictions between sources (different dates, titles or employers on the CV and on LinkedIn,
  overlapping jobs). Never pick one silently.
- Missing facts: exact dates, location, full URLs, numbers behind vague claims ("reduced downtime" by
  how much?), what a project is used for and by whom.
- How each recent job ended, if the CV will raise the question (short tenure, gap). This is for the
  interview answer, not for the CV.

## 4. Critique honestly

Before rebuilding, tell them what you would change and why: what to cut, what to merge, what to move
up, what is missing. Do not agree with everything they wrote. Disagree once, clearly, then follow
their decision.

## 5. Write, compile, check

1. Copy `template/harvardcv.sty` next to the new `.tex`. Start from `template/example-cv.tex`.
   With several versions, put the header in a shared `contact.tex` and `\input` it.
2. Write each line following `references/writing-guide.md`.
3. Compile with `xelatex` (twice if links or layout look off). The font is TeX Gyre Termes, which
   ships with TeX Live and MiKTeX. Without a local TeX install, tell them to upload the folder to
   Overleaf and set the compiler to XeLaTeX.
4. Check, every time:
   - Page count (`pdfinfo`): exactly the limit.
   - Line wraps (`pdftotext -layout`): a bullet that spills one or two words onto a new line gets
     shortened until it fits on one line.
   - A rendered preview (`pdftoppm -png -r 80`) for spacing and alignment.
5. If it overflows: cut weak bullets first, then merge lines, then collapse old jobs into one-line
   entries. Shrink margins or font size last, and never below 0.4in margins or 10pt.

Deliver the PDF and the `.tex`. Keep iterating on their feedback; recompile and recheck after each change.

## 6. After the CV

If a job on the CV ended in a layoff, a firing or a short contract, offer to prepare the interview
answer (section "Explaining how a job ended" in the writing guide).
