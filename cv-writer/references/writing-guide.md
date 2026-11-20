# CV writing guide

Rules learned from rebuilding real CVs (engineering, software, customer service, project management, in
English and Spanish). Each rule says what to do and why.

## Format (Harvard style)

- **One page.** Recruiters skim for seconds. Two pages only for long senior careers or academic CVs.
- **Reverse chronological order** inside every section, by start date. A newer job listed below an older
  one reads as a mistake.
- **No photo, no "profile" or "objective" paragraph.** A one-line subtitle under the name does the same
  job in a tenth of the space: `Software Engineer | ICPC World Finalist`,
  `Mechanical Engineer | Project Manager`.
- **Sections, in this order:** Experience, Projects (if relevant), a section for the differentiator
  (competitions, publications, certifications), Education, Skills. Recent graduates may put Education
  first.
- **Each role:** organization in bold with dates on the right; title in italics with location on the
  right. Old or minor jobs collapse into one line (`\shortrole`), optionally under "Earlier experience".
- **Header:** name, subtitle, city and country, phone with country code, email, full LinkedIn URL
  (`linkedin.com/in/...`, never "LinkedIn: Name"), GitHub, portfolio. Language levels can go in the
  header or in Skills, once.
- **Paper:** Letter for the US and Canada, A4 elsewhere. Margins 0.4–0.5in, body 10–11pt.

## Bullets

- **Start with a past-tense action verb** (present tense only for the current job): Built, Led,
  Maintained, Negotiated, Diagnosed. Not "Responsible for", not "Worked on", not a noun phrase.
- **What you did, how, and the result.** Put a number on it whenever one exists (6 concurrent projects,
  $2M pipeline, 95% SLA compliance, 200+ tests). Ask for the number; never invent one.
- **One line per bullet.** If it wraps by a word or two, cut words until it fits. Two lines only when
  the second line carries real information.
- **2–3 bullets for recent, relevant jobs; 1–2 for older ones; none for jobs that are only dates.**
  The most relevant job for the target role gets the most space, even if it was short.
- **No bold label prefixes** ("**SLA Management:** Handled…") and no parenthetical self-assessment
  ("Transferable skill: high problem-solving ability…"). They take space and read as filler.
- **No buzzwords** ("drastically", "cutting-edge", "solid track record", "dynamic"). Write it the way the
  person would explain it to a colleague. Plain verbs beat adjectives.
- **Don't repeat the stack.** A bullet that only lists technologies ("Worked with C++, Python, Docker…")
  duplicates Skills; delete it and keep the tools inside the bullets where they did something.

## Projects

- One or two lines each: what it is, who uses it, and the engineering signals a reviewer looks for
  (auth, tests, CI, deployment, a real user or client).
- Cut domain details only an insider understands, internal version numbers, and migration tools; the
  stack already sits in the project's title line.
- Mark a project "(freelance)" only when there is a client. A real client or real usage ("used at a
  120-athlete tournament") is worth more than the label.
- A current project with dates "… – Present" covers a gap after the last job.

## Tailoring to a target role

- Same facts, different emphasis: reorder bullets, choose which lead, rename the subtitle. Never change
  the facts between versions.
- For a backend role, lead with APIs, data, integrations and deployment; for management, with scope,
  budget, deadlines and stakeholders; for customer service, with SLAs, languages and tools.
- The differentiator should be visible in five seconds (subtitle plus a short section) but should not
  take most of the page. Three bullets is usually enough for a strong competition record.

## Honesty

- **Never lie.** Every line must survive "tell me more about this" in an interview.
- **Dates are facts.** Never stretch or merge them to hide a gap. Background checks verify them. If a
  job was interrupted, show both periods (`Jan 2021 – Jun 2021, Feb 2022 – Dec 2022`).
- **Courses in progress** are allowed only when labeled: `Claude API and MCP (in progress)`. Do not list
  planned courses.
- **Location is where the employer is based** (or `Remote (US)` when remote for a US company). Do not
  pick a country because it sounds better.
- **Titles** must match what the employer or LinkedIn says. If they differ, ask which is right.
- Short contracts: label them "(Freelance)" or "(Contract)" when true; it explains the short duration.

## Certifications and courses

- List completed certificates that matter for the target role; drop the rest. "Dozens of modules on online
  platforms" is noise.
- Merge certificates from the same platform and year into one line:
  `Google Project Management and IBM IT Project Manager Professional Certificates, Coursera — 2025`.
- An approved exam application with a date is fine: `PMP: application approved by PMI — exam Mar 2027`.
- A certificate that proves a tool goes next to the tool in Skills: `Claude Code (Anthropic Academy certified)`.

## Education

- Degree, institution, graduation date, one line each.
- Add a thesis title and honors when notable (highest honors, top grade).
- Include technical or vocational degrees; they show depth in engineering trades.

## Skills

- 3–5 labeled lines (Programming, Backend, DevOps, Tools, Languages). Each line fits on one line.
- Languages with a level and, if available, the test: `English (C1, EF SET)`.

## Spanish and other languages

- For Spanish, load `\usepackage[spanish,es-noshorthands,es-nolists]{babel}`: the options keep `~`, `<`,
  `>` and itemize bullets working normally.
- Translate section names (Experiencia Profesional, Formación Académica, Certificaciones, Habilidades)
  and month abbreviations (Ene, Abr, Ago, Dic). Keep official English names of certificates.

## Explaining how a job ended

The CV never says why a job ended. Keep relevant jobs even if they ended badly: removing them loses
experience and opens a gap that needs explaining anyway.

For the interview, prepare a short answer with three parts: one honest sentence on why it ended, what
was learned, what the person does now. No blaming the employer, no invented reasons (employers
sometimes call to check). Examples:

- **Layoff:** "The company restructured and my position was cut. It wasn't performance-related."
- **Performance:** "They expected faster ramp-up than I delivered at first. I learned to clarify
  requirements early and flag blockers sooner, and that's how I work now."
- **Fit:** "It wasn't the right fit: they needed someone more customer-facing, and I'm strongest on the
  engineering side, which is what I'm looking for now."
- **Probation:** "They decided not to continue after the trial period. The feedback was [X], and I've
  worked on it since."

Close with the present: "Since then I've been building [project] for [client]."

## Final checks

- Page count equals the limit; no bullet wraps by one or two words.
- Dates in reverse chronological order, no unexplained overlaps.
- Every URL is full and clickable; email and phone are correct.
- Nothing claimed that the person could not explain in an interview.
