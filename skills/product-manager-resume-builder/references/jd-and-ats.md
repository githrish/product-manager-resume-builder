# Reading a job description, and surviving the parser

Read this in Phase 5, before scoring a match or finalising a version.

## Classifying requirements

Not every line in a posting carries the same weight. Sort them before scoring, because a match percentage that counts nice-to-haves the same as must-haves is misleading.

**Treated as required** when the posting says must have, required, essential, or you have; when it sits under a Requirements heading; or when the same idea appears three or more times anywhere in the text.

**Treated as preferred** when the posting says nice to have, bonus, a plus, ideally, or preferred; or when it appears only once or twice.

Repetition is the most reliable signal and the most often missed. If a posting mentions experimentation in the summary, in the responsibilities, and again in the qualifications, it is a must-have regardless of which heading it sits under.

## Dealbreakers, and things that only look like dealbreakers

Tell the candidate plainly which is which. Talking someone out of a winnable application is as costly as encouraging a hopeless one.

**Genuine dealbreakers.** A licence or certification they do not hold when it is stated as required. Security clearance they cannot obtain. Work authorisation for the market. A hard location requirement they cannot meet. Years of experience more than about half below the stated bar.

**Not dealbreakers, apply anyway.** Years slightly below the bar, such as three when the posting asks for five. A preferred degree they do not have. Tools and platforms they could learn in a fortnight. Industry experience when the transferable case is strong. Almost every posting is a wish list, and the median hire misses several lines on it.

For PM postings specifically, treat these as soft: a named analytics tool, a specific framework, and "MBA preferred". Treat these as hard: domain experience in regulated areas, and any explicit technical bar such as reading SQL or working with APIs, where the interview will test it directly.

## Reading the posting for what it does not say

- **A vague posting** usually means the team has not agreed on the role. Expect the interview loop to be inconsistent and the scope to shift after joining
- **A very long requirements list** often means several stakeholders each added their own line. Prioritise the first third; it is usually written by the hiring manager
- **A wide salary band** normally signals flexibility on level, which is useful for a transitioner. It can also mean they have not decided what they need
- **Repeated mentions of pace, ownership, or ambiguity** describe a small or under-resourced team. Fine if that suits the candidate, worth naming if it does not
- **Named tools** suggest an operationally mature team. Their absence suggests the opposite
- **No mention of who the role reports to** is worth asking about in a first call

Before applying, it is worth checking recent company news for layoffs or funding, and how long people stay in similar roles. Say this once as advice; do not turn it into a research project inside a resume session.

## ATS parser failures

Keyword matching only happens after the file parses. Most rejections that people blame on keywords are parse failures. The formatting spec in the templates reference prevents nearly all of them, but check these explicitly before finalising:

- **Multi-column layouts** read left to right across both columns and interleave the text into nonsense
- **Tables** frequently lose their structure, and a table used for contact details can drop the details entirely
- **Text boxes and shapes** are often skipped completely, so anything inside one disappears
- **Headers and footers** are ignored by many parsers, which is why contact details must sit in the body
- **Images and logos** contribute nothing, and a resume built as an image contributes nothing at all
- **Non-standard bullet glyphs and decorative dividers** can turn into replacement characters
- **Unusual section headings** such as "Where I've been" are not recognised as Experience
- **Dates in inconsistent formats** confuse duration calculations, which some systems use to filter by years of experience
- **A PDF exported from a design tool with text converted to outlines** contains no text at all

**The check that catches all of it.** Open the finished PDF, select all, copy, and paste into a blank document. What appears is approximately what the parser sees. If the order scrambles, if anything vanishes, or if characters come through wrong, fix it before sending. This takes under a minute and is the single highest-value formatting check available.

## Scoring the match

```
Match score = required keywords present ÷ total required keywords × 100
```

Count only the required set. Report the number, then interpret it:

- **85% and above.** Strong fit. Apply, and spend the saved effort on a referral
- **70 to 84%.** Worth applying. Name the gaps and how to cover them
- **55 to 69%.** A stretch. Worth it only with a referral or a genuinely strong adjacent case
- **Below 55%.** Say plainly that the resume is not the problem. Either the target is wrong or the evidence needs to be built first

Never inflate the score by counting preferred items, and never suggest adding a keyword for something the candidate has not done.
