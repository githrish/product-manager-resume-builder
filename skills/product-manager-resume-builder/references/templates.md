# Templates, rendering, and the final file

Read this at step 5, before offering a layout, and again at step 6 when producing the deliverable.

## What ATS safety actually forbids

Get this right or the rest does not matter. Parsers fail on **structure**, not on styling.

**Breaks parsing:** multiple columns, tables, text boxes, images, icons, logos, charts, headers and footers, text converted to outlines, anything where reading order is not top to bottom.

**Parses fine:** colour, bold and italic, font choice and size, letter spacing, horizontal rules, generous whitespace, links, small caps, uppercase section headers.

So the resume can look designed. It cannot look like a Canva template with a sidebar. Every layout below is single column, real selectable text, top-to-bottom reading order.

## Show it before they choose

**Never ask someone to pick a layout from a description.** Skeletons and bullet lists do not tell anyone what their resume will look like.

At step 5, render the top third of the page in **every** layout using the candidate's real content, side by side, and let them look. The top third is where the decision lives, since the body is nearly identical across layouts.

Produce this as a single HTML file they can open, or as an inline preview if the interface renders one. Say two things alongside it: that the summary is a draft and not locked, and that anything rendering in sentence case here will be uppercase in the final file.

If the environment truly cannot render anything, say so plainly and paste the top third of each layout as preformatted text. That is a degraded experience, not the intended one.

## The five layouts

All are one page, single column, and use fonts that exist on both macOS and Windows so the PDF and the DOCX look the same. Sizes are for a one-page target; scale the body by half a point either way to fit.

### 1 · Classic

Conservative and quiet. The safest choice for banks, enterprise, consultancies, and any large company with a strict process.

```
Font          Georgia (headings) + Georgia (body)
Name          20pt, regular, letterspacing 0.02em
Section head  10pt, uppercase, letterspacing 0.18em, 1px rule below, full width
Role line     11pt bold, company and dates on the same line, dates right-aligned
Context line  9.5pt italic, grey 40%
Body          10pt, leading 1.35
Accent         none, black and greys only
Margins       0.6in
```

### 2 · Modern

Sans throughout, one accent colour, generous air. The default for startups, product companies, and most PM roles.

```
Font          Calibri, or Helvetica Neue where available
Name          22pt, semibold, letterspacing -0.01em, accent colour
Section head  9.5pt, uppercase, letterspacing 0.2em, accent colour, 1px rule below in 15% accent
Role line     11pt semibold; dates 10pt regular, grey 45%, right-aligned
Context line  9.5pt, grey 45%
Body          10pt, leading 1.4
Accent        one colour only, a deep blue or slate. Never on body text
Margins       0.55in
```

### 3 · Compact

For candidates with a lot of material: eight or more years, or three roles plus projects. Buys roughly six extra lines without dropping to unreadable type.

```
Font          Calibri
Name          18pt, semibold
Section head  9pt, uppercase, letterspacing 0.16em, rule below
Role line     10.5pt semibold, dates inline after a pipe
Context line  9pt, grey 45%
Body          9.5pt, leading 1.28
Accent        optional, section heads only
Margins       0.45in
```

### 4 · Editorial

A large name, a strong rule, and room to breathe. Suits senior and lead candidates whose page has fewer, heavier bullets.

```
Font          Georgia (name and section heads) + Calibri (body)
Name          28pt, regular, letterspacing -0.015em
Contact       9.5pt, directly under the name, pipe separated
Rule          2px full width under the contact block, accent colour
Section head  10pt, uppercase, letterspacing 0.2em, no rule
Role line     11pt bold
Body          10pt, leading 1.45
Accent        one colour on the rule and the name only
Margins       0.65in
```

### 5 · Minimal

No colour at all. Pure typographic hierarchy. Prints identically anywhere and survives the worst parsers.

```
Font          Helvetica or Arial
Name          19pt, bold, uppercase, letterspacing 0.05em
Section head  9.5pt, bold, uppercase, letterspacing 0.15em, no rule, extra space above
Role line     10.5pt bold
Context line  9.5pt, grey 50%
Body          10pt, leading 1.4
Accent        none
Margins       0.6in
```

## Section order

| Situation | Order |
|---|---|
| PM with PM experience | Contact, summary, experience, skills, education |
| Switching in from another function | Contact, summary, experience reframed, projects, skills, education |
| Breaking in early career | Contact, summary, projects, experience, skills, education |
| Recent graduate | Contact, summary, education, projects, experience, skills |

## Building the final file

The deliverable is a **PDF and a DOCX**, not Markdown. Markdown is a staging format only, and it is shown to the candidate at step 5 as part of the layout review, never handed over as the finished resume.

**Author in HTML.** It is the only format where line widths can be measured, which is what the 80% line-fill rule needs. Write a single self-contained HTML file with a print stylesheet:

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

Expect to tune spacing per layout. Identical content ran 31 to 62px long across these five layouts before adjustment, because their type scales differ. Each layout needs its own section gaps and bullet spacing to land on the same line.

## Before handing it over

- Every bullet fits two rendered lines or fewer
- Every wrapped bullet fills at least 80% of its last line
- Numbers and outcome phrases are bold, two spans per bullet at most
- One page, without shrinking margins below 0.4in or body text below 9.5pt
- Copy the text out of the finished PDF and paste it into a blank document. That is what the parser sees. If the order scrambles or anything vanishes, fix it before sending
- File named `First_Last_Resume.pdf`
