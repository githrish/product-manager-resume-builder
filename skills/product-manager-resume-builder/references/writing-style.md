# Writing style: sounding like the candidate, not like a model

Read this at step 4, before writing any bullet, and again at step 6 as a check.

A resume that reads as machine-written costs the candidate credibility at exactly the moment they need it. Recruiters see hundreds of these a week and have become good at spotting them. The tells below are what give it away.

## The tells, in order of how much damage they do

**1. Trailing participle clauses.** This is the strongest signal and the easiest to produce by accident. State a fact, then bolt on an "-ing" phrase to make it sound deeper.

- Wrong: Launched paid access in April, **driving** 9 paying customers and **establishing** early revenue
- Right: Launched paid access on 21 April. First sale in 12 hours, 9 paying customers to date

Scan every bullet for a comma followed by an "-ing" word. Almost all of them should be cut or turned into a second clause with a real verb.

**2. Em dashes and en dashes.** Use a comma, a semicolon, a colon, a full stop, or a pipe in a header line. Never `—` or `–` anywhere in the document.

**3. Stacked ownership verbs.** "Spearheaded end-to-end ideation and launch of" is three claims doing one job. One verb, then the facts.

**4. Forced groups of three.** Real work rarely comes in tidy triples. If a bullet lists exactly three things and the third is weak, it was added for rhythm. Cut it.

**5. Inflated abstractions.** Strategic, holistic, robust, seamless, comprehensive, leveraged, spearheaded, orchestrated, pivotal, key. Replace with what actually happened.

**6. Sales register.** "Passionate about building delightful experiences" belongs on a landing page, not a resume.

**7. Symmetrical bullets.** If every bullet in a role has the same shape, verb, clause, metric, the section reads as generated. Vary the structure. Some bullets end on the decision, some on the number, some on the constraint.

**8. Vague intensifiers.** Significantly, substantially, dramatically, considerably. Either you have the figure or you do not.

## The positive test

Read the bullet aloud. If it sounds like something the candidate would say in an interview, it is right. If it sounds like something written *about* them, rewrite it.

The candidate's own phrasing from step 3 is usually better than anything polished. When they said "not chasing the supply side and bringing it with cross-compatibility had us in a much better state to scale through ads", the resume line should keep that thinking, tightened, not replace it with "leveraged cross-platform compatibility to optimise supply-side acquisition".

## Bullet length and line fill

Two hard rules, both about how the page looks before anyone reads it.

**No bullet runs past two rendered lines.** Three-line bullets are skipped. If it needs three lines, it contains two ideas: cut one or split it.

**No wrapped bullet ends its last line under 80% of the text width.** A two-line bullet whose second line holds two words looks broken and wastes the row. Fix it one of two ways:

- **Tighten to one line.** Usually possible by cutting a qualifier or a redundant clause.
- **Expand to fill.** Add a real detail the candidate gave you: team size, timeframe, the constraint, the rejected option. Never filler words.

This can only be enforced against a rendered document, not against Markdown, since Markdown has no line width. Measure at step 5 when the layout exists, and again after any edit.

### How to hit it, rather than guess at it

Measure the chosen layout's **characters per line** first. Render one long bullet, count its characters, divide by the number of visual lines it occupies. Call that `c`.

Then every bullet must land in one of two windows:

- **One line:** at most `0.95 c` characters
- **Two lines:** between `1.82 c` and `1.99 c` characters

Anything between those two windows is the dead zone. A bullet at `1.4 c` wraps to two lines and leaves the second one 40% full, which is the exact defect this rule exists to prevent.

Write to the character count. It is faster and far more reliable than writing a bullet, rendering it, and nudging words until it looks right.

Two consequences worth knowing:

- **The window is layout-specific.** A serif at 10pt holds around 107 characters per line; a narrow sans like Calibri holds around 120 in the same measure. The same sentence that fills two lines perfectly in one layout leaves an orphan in the other. Retune whenever the layout changes.
- **Overshooting is worse than undershooting.** A bullet slightly too long spills to three lines with a near-empty tail. A bullet slightly too short simply sits on one line, which is always acceptable.

## Bolding for skimmability

Recruiters scan before they read. Bold gives them landing points.

**Bold the number and the two or three words naming what it moved.** Roughly two bold spans per bullet, never more.

- Grew DAU for Student Practice Questions **from 20K to 100K+** in 4 months with notification campaigns and A/B tests
- Owned the iOS launch end to end with 2 engineers, QA and an analyst; **0 to Rs 1M/day revenue in 6 months**

Do not bold verbs, tool names, skill words, or whole clauses. A page where a third of the text is bold has no emphasis at all. If a bullet has no number, it usually needs no bold.
