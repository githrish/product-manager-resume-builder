# Templates, rendering, and the final file

Read this at step 5, before offering a layout, and again at step 6 when producing the deliverable.

## What ATS safety actually forbids

Get this right or the rest does not matter. Parsers fail on **structure**, not on styling.

**Breaks parsing:** multiple columns, tables, text boxes, images, icons, logos, charts, headers and footers, text converted to outlines, anything where reading order is not top to bottom.

**Parses fine:** colour, bold and italic, font choice and size, letter spacing, horizontal rules, generous whitespace, links, small caps, uppercase section headers.

So the resume can look designed. It cannot look like a Canva template with a sidebar. Every layout below is single column, real selectable text, top-to-bottom reading order.

## Two decisions, not one

Step 5 has a **structure** and a **treatment**, and they are decided by different people.

**You pick the structure**, from what step 2 established. Three are available: experience-first, education-first, multi-role. The candidate has the least information about this and the most to lose by guessing: someone breaking into product who picks an experience-first layout buries the projects that are their whole case. State which structure you chose and why, in one line, and let them override.

**They pick the treatment.** Once the structure is right, what remains is typography and density, which is a matter of taste and theirs to decide.

## The structures

### Experience-first

The default. For anyone with professional experience worth leading on, including switchers coming in from another function.

```
Contact  →  Summary  →  Experience  →  Skills  →  Education
```

Switchers use the same shape with the bullets reframed around product decisions, and a Projects section after Experience when their strongest evidence sits outside the day job.

### Education-first

For students, recent graduates, and anyone with under about two years of work. Education carries real weight early on and then stops mattering almost entirely, so it leads here and nowhere else.

```
Contact  →  Education  →  Experience  →  Projects  →  Skills
```

Three things change beyond the order:

- **Education carries detail** it would never carry later: degree and institution, graduation year, GPA or CGPA where the market expects it, honours, and relevant coursework when the role is technical. Two to four lines, not one.
- **Projects becomes a real section**, each with a name, a date, and one or two bullets. For someone with no PM title this is often the strongest evidence on the page, and it must not sit below a thin work section.
- **The company gets a descriptor**, inline and in parentheses: `NORTHWIND (8-person venture-backed payments startup)`. An early-career candidate's employers are usually unknown to the reader, and the descriptor supplies the scale their bullets are measured against.

Summary is optional here. A student with three lines of genuine positioning should keep it; one padding it with adjectives should drop it and use the space on projects.

### Multi-role

For a candidate promoted inside one company, or whose work is better told by project than by job title. Common in PM: APM to PM at the same employer, or three years across four product areas under one heading.

```
Contact + current title  →  Experience (company once, roles nested)  →  Education  →  Additional information
```

What changes:

- **The current title goes under the name**, on its own line. It tells the reader what you are before they reach the first role, which matters when the roles beneath are plural.
- **The company appears once**, with locations right-aligned. Each role sits beneath it as a title with its own date range, most recent first. Do not repeat the company or restate its description; the progression is the point and repeating the employer hides it.
- **Bullets belong to the company, not the role**, unless a specific achievement clearly belongs to one title. Splitting three bullets across two roles usually leaves both looking thin.
- **A project sub-block** can sit inside a role: a "Selected Project Experience" heading, then named projects each carrying their own bullets. Use it when the work groups more naturally by initiative than by year.
- **Additional Information** replaces the skills rows: technical skills, certifications and languages as labelled lines.

Reach for this only when there is real progression or genuine project grouping to show. With one role at one company it adds structure and says nothing.

## Show it before they choose

**Never ask someone to pick a layout from a description.** Skeletons and bullet lists do not tell anyone what their resume will look like.

Render the top third of the page in **every** treatment using the candidate's real content and the structure you selected, side by side, and let them look. Produce it as a single HTML file they can open, or as an inline preview if the interface renders one.

Say two things alongside it: that the summary is a draft and not locked, and that anything rendering in sentence case here will be uppercase in the final file.

If the environment truly cannot render anything, say so plainly and paste the top third of each as preformatted text. That is a degraded experience, not the intended one.

## Which structure for whom

| Step 2 track | Structure | Why |
|---|---|---|
| Holds a PM title | Experience-first | The roles are the case |
| Switching in, 3+ years elsewhere | Experience-first, bullets reframed, Projects after Experience | Seniority is real and must not be buried behind education |
| Early career, under 2 years | Education-first | Education and projects are the strongest evidence available |
| Student or recent graduate | Education-first | Same, with coursework and honours carrying weight they never will again |
| Promoted within one company, or project-shaped work | Multi-role | The progression is the strongest signal and a flat list of jobs hides it |

When a candidate sits on the boundary, ask rather than guess: "Is your degree or your work the stronger part of your case right now?"

## The five treatments

Every one is single column with real selectable text. What varies is typeface, whether section headers are ruled, and density. All of them render either structure.

### 1 · Classic

Serif throughout, ruled headers. The safest choice at banks, consultancies, and anywhere the process is old and strict.

```
Font          Georgia
Name          27px, regular, letterspacing 0.02em
Section head  12.8px, uppercase, letterspacing 0.18em, 1px rule below
Role line     14.4px bold, dates right-aligned
Context       12.4px, grey 43%
Body          12.9px, leading 1.43
Accent        none
Margins       46px vertical, 43px horizontal
```

### 2 · Modern

Sans with section headers in a muted blue, the only colour on the page. The default for product roles.

```
Font          Calibri, or Carlito where Calibri is absent
Name          29px, semibold, letterspacing -0.01em
Section head  12.4px, uppercase, letterspacing 0.2em, #3A6EA5, rule below at 28% tint
Role line     14.4px semibold, dates right in grey
Body          13.3px, leading 1.41
Accent        #3A6EA5, headers only, never on body text
Margins       46px / 48px
```

### 3 · Structured

The LaTeX shape most candidates recognise from Overleaf: centred header, small-caps rules, and a two-row entry.

```
Font          Times New Roman
Name          31px, regular, centred; contact centred beneath, pipe separated
Section head  13.4px, small-caps, 1px rule below
Entry         role bold left with dates right, then company italic left with location right
Body          13.2px, leading 1.38
Accent        none
Margins       44px / 46px
```

### 4 · Compact

Tightened margins and type for candidates carrying eight or more years, or a long projects section.

```
Font          Calibri or Carlito
Name          25px, semibold
Section head  12.2px, uppercase, letterspacing 0.16em, rule below
Body          13.6px, leading 1.39
Accent        none
Margins       46px / 52px
```

### 5 · Bold

The heaviest of the five. Centred name with the current title on its own line beneath it, uppercase ruled sections, and bold on every company and role line, so the page scans in a single pass. Suits a candidate whose titles and employers are the strongest thing on the page, and it is the natural partner for the multi-role structure because nested role lines need weight to stay legible.

```
Font          Arial or Helvetica
Name          24px, bold, uppercase, centred
Title line    15.5px, bold, centred, directly under the name
Section head  12.6px, bold, uppercase, rule below
Body          12.8px, leading 1.42
Accent        none
Margins       44px / 46px
```

Editorial, a large serif name over an accent rule, was dropped in its favour. It read as a variation on Modern rather than a real alternative.

## Building the final file

The deliverable is a **PDF and a DOCX**, not Markdown. Markdown is a staging format only, and it is shown to the candidate at step 5 as part of the layout review, never handed over as the finished resume.

**Author in HTML.** It is the only format where line widths can be measured, which is what the line-fill rule needs. Write a single self-contained HTML file with a print stylesheet:

```css
@page { size: A4; margin: 0; }
body { margin: 0; }
.page { width: 210mm; min-height: 297mm; padding: <margin from the layout>; }
```

Use A4 for India, the UK, Europe and most of the world. Use US Letter (216mm by 279mm) for the US and Canada.

**Then convert.**

- **PDF:** print the HTML to PDF from a browser, or use a headless converter if one is available. Keep text selectable. Never export with text as outlines.
- **DOCX:** produce it from the same content with whatever the environment provides, `pandoc` or a document library. If nothing is available, say so and hand over the HTML and PDF, telling the candidate to open the HTML in Word and save as .docx.

**If the environment cannot run code at all**, output the complete HTML in a code block with instructions: save as `resume.html`, open in a browser, print to PDF. Do not pretend a Markdown file is the deliverable.

## Filling the page top to bottom

A resume that stops two thirds down the page reads as thin, whatever the content says. Target the content ending within about 10px of the bottom margin, so the text block is genuinely full.

Measure it as `content bottom` against `page height minus bottom margin`. Do not measure against the page height itself, which ignores the margin and lets the text run into it.

When there is space left over, in this order. The order is the point: the first move adds evidence, the last only adds air.

1. **Restore something you cut.** A bullet dropped earlier for space beats any amount of extra leading.
2. **Ask for one more achievement.** Go back to the candidate rather than stretching what is already on the page.
3. **Expand a bullet from one line to two**, but only where a real detail was left out. Never to reach a length.
4. **Open up the spacing.** Section gaps and leading, in small increments.

Never lengthen sentences to fill a page. A short bullet with a number beats a long one padded to the margin, and the padding is visible to anyone who reads carefully.

When the content overruns, reverse the order: tighten spacing first, shorten bullets second, and only cut a bullet as a last resort.

Expect to tune spacing per treatment. Identical content ran 31 to 62px long across the treatments before adjustment, because their type scales differ. Each needs its own section gaps and bullet spacing to land on the same line.

## Before handing it over

- Every bullet fits two rendered lines or fewer
- No wrapped bullet strands its last line below roughly 30% of the width
- The summary, skills rows and education line clear the same floor, since short rows there are the most common way a page looks unfinished
- No metric, scope figure or decision was cut to make a line end tidily
- Numbers and outcome phrases are bold, two spans per bullet at most
- One page, without shrinking margins below 0.4in or body text below 9.5pt
- Copy the text out of the finished PDF and paste it into a blank document. That is what the parser sees. If the order scrambles or anything vanishes, fix it before sending
- File named `First_Last_Resume.pdf`
