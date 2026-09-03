# Bullet mechanics

Read this at step 4, before writing any bullet.

### The PM bullet formula

```
[Ownership verb] [what you shipped or decided] for [who / what scale],
[measurable outcome] by [the non-obvious method]
```

The last clause is the one PMs skip, and it's the one that proves you did the work rather than sat near it.

**Before:** Owned the roadmap for the merchant dashboard
**After:** Rebuilt the merchant dashboard roadmap around three retention bets, lifting 90-day merchant retention from 61% to 74% by cutting six planned features that user interviews showed nobody used

### The outcome test, run it on every bullet before anything else

Read the bullet and ask **so what happened?** If the answer is not in the bullet, the bullet is not finished. This is the single check that catches the most failures, and it outranks every other rule here.

A bullet may describe an action, a decision, a method, or a launch. None of those is an outcome. "Launched X before Y to prove Z" states a sequence and stops. "Migrated the service to a new queue" states a task. Both pass every anti-pattern below and both are still dead, because a reader finishes them and knows nothing about what changed.

Three ways out, in order of preference:

1. **Add the result.** Usually it exists and was left out because it felt obvious to the person who lived it.
2. **Merge it into the bullet it serves.** A method with no result of its own is often the missing `by doing Z` clause of the bullet above or below it. Two half-bullets make one strong one, and you get a line back.
3. **Cut it.** A resume with six bullets that each land beats one with ten where four are scaffolding.

Never solve this by adding a number that was not measured. Never solve it by inflating the verb, which is the most common repair and the most transparent.

### Verbs, the smallest lever on the page

Open every bullet with a verb that names what you actually did. That much is settled. The part most advice gets wrong is what "strong" means.

**Weak openers, rewrite these.** *Built, worked on, helped, supported, assisted, participated in, involved in, responsible for, tasked with, contributed to.* They either describe proximity to the work rather than ownership of it, or they are so general that they carry no information. *Built* is the one that slips through most often, because it sounds concrete while saying nothing about your role.

**Inflated openers, also rewrite these.** *Spearheaded, orchestrated, revolutionised, transformed, pioneered, championed, drove, leveraged, engineered the development of.* Recruiters read these as filler rather than as signal, and an experienced one reads the gap between an inflated verb and a thin outcome instantly. On a junior resume they actively cost credibility. Reaching for a thesaurus is a sign the underlying bullet is weak; fix the bullet instead.

**What to use.** The plain verb that describes the actual act: *owned, shipped, launched, rebuilt, cut, raised, migrated, priced, negotiated, instrumented, killed, scoped, replaced, ran*. Specific beats impressive. *Killed three features nobody used* is stronger than *streamlined the product portfolio* and always will be.

**Do not repeat a verb inside one role**, and do not stack two (*designed and implemented*). Pick the one that carries the weight.

### The Ownership Ladder, pick the honest rung

| Verb | Means | Only use if |
|---|---|---|
| **Owned / Led** | You were accountable; the outcome was yours | You'd be the one fired if it failed |
| **Drove** | You set direction and pushed it through others | You made the call but shared accountability |
| **Partnered with / Worked with X to** | Genuine joint ownership | Another function co-owned the decision |
| **Contributed to / Supported** | You did real work on someone else's thing | You weren't setting direction |

Never upgrade a rung to sound better. An interviewer's second question always exposes it.

### The PM metric taxonomy

When a bullet needs a number, pull from the category that matches the archetype:

- **Adoption**, users activated, % of eligible accounts using it, teams onboarded, time-to-first-value
- **Retention**, D1/D7/D30, cohort curves, churn rate, renewal/expansion
- **Engagement**, sessions, depth per session, feature usage frequency, DAU/MAU ratio
- **Revenue**, ARR/MRR influenced, conversion rate, ARPU, take rate, deal size
- **Efficiency**, cost saved, support tickets deflected, manual hours removed, infra cost
- **Quality**, bug/incident rate, latency, uptime, CSAT/NPS, error rate
- **Velocity**, release frequency, cycle time, experiments run per quarter, time-to-decision

**Scale counts as a metric.** "Across 12 enterprise accounts" or "for a 40-person eng org" gives a hiring manager the calibration they need even with no delta.

### The Estimation Protocol, for when they have no numbers

Never skip a metric, and never fabricate one. Instead:

1. **Find the anchor.** "How many customers did your product have?" / "What was team headcount?" / "How many tickets came in weekly?" People know these even when they don't know outcomes.
2. **Reason to a range with them, out loud.** "If support was handling ~200 tickets a week and this removed the top reason for contacting, that's plausibly 15–25% deflection. Does that match what you saw?"
3. **Land on the conservative end.** Always.
4. **Label it.** Mark every estimated figure `[EST]` in the working draft, and tell them: *"You'll need to be ready to explain how you arrived at this. If you can't, we cut it."*
5. **Offer the hedge.** "~", "over", and "roughly" are honest and interviewers accept them.

### PM resume anti-patterns, flag these on sight

- **"Responsible for the product roadmap"**, describes the job title, not the person
- **"Worked cross-functionally with engineering and design"**, this is the definition of PM; it's not an achievement
- **"Gathered requirements from stakeholders"**, reads as order-taker, the single most damaging PM resume phrase
- **"Agile/Scrum/Jira/Figma"** listed as skills, these are table stakes and burn credibility as differentiators
- **Feature lists**, "Launched dark mode, notifications, and SSO" with no outcome is a changelog
- **Team results as personal claims**, "Grew revenue 40%" when you owned one feature in that funnel
- **Vanity metrics with no baseline**, "increased engagement 200%" from a base of 3 users
- **Certifications as headline**, CSPO/PSPO in the summary signals you're compensating for thin experience
- **The scope inventory**, "Built the product end to end, from onboarding through payments and analytics" lists everything you touched and reports nothing that happened. Breadth is context, never the achievement. If solo scope is genuinely the point, count it and attach a result: *shipped all five systems alone and reached paying customers with no engineering hire*
- **Claims of absence**, "with no engineering help", "with zero budget", "single-handedly", "with no design support". You cannot verify an absence and neither can the candidate, so it reads as a boast the moment anyone probes it, and one contractor or one weekend of help from a friend makes it false. Never write one the candidate did not state in their own words, and when they do state it, ask what help they actually had before it goes on the page. Founders and solo builders almost always had more help than they remember at intake.
- **Solo repeated**, once the role line says founder or sole owner, the bullets do not need to say it again. Three assertions of working alone in one section reads as insecurity about the scope rather than as evidence of it. State it once, in the role descriptor, and let the ownership verbs carry the rest
- **The orphan method**, a decision or sequence with no consequence attached. See the outcome test above; merge it or cut it
- **Someone else's number**, a product-wide NPS or a company revenue figure sitting at the end of a bullet about your feature. It reads as borrowed the moment anyone asks about it in an interview

**Additional anti-patterns when breaking in**

- **"Aspiring Product Manager" as a headline**, it announces what you are not. Name your real function and the direction you're moving.
- **A retitled past job**, see the Title Honesty Rule. Verified, and offer-losing.
- **Coursework listed as experience**, a class is not a shipped product
- **A wall of certifications**, five PM certificates read as a substitute for evidence, not a supplement to it
- **"Passionate about products"**, every applicant writes this
- **Teardowns of famous apps in the Experience section**, excellent in a portfolio, disqualifying as work history
- **No evidence of ever shipping anything**, if this is genuinely true, run the Gap-Filling Sprint at steps 2 and 6


### The bullet audit, run at step 6

Score every bullet against five checks and show the candidate the failures. Do not silently rewrite.

| Check | Passes when |
|---|---|
| **Outcome** | A reader knows what changed. Not what you launched, ran, or decided |
| **Measure** | A number, or an explicit scale figure where no delta was ever measured |
| **Method** | The non-obvious thing you did, so the outcome is credibly yours |
| **Verb** | Specific and accurate. Not on the weak list, not on the inflated list, not repeated inside the role |
| **Ownership** | The claim matches the rung on the Ownership Ladder. No borrowed numbers, and no claim of absence the candidate did not make themselves |

**Reporting it.** Say how many bullets failed and on which check, name the worst two, and give the rewrite alongside the original so the candidate can see the difference. A resume where every bullet passes all five is rare and usually means someone padded; two or three honest misses in a first draft is normal. What is not acceptable is shipping a bullet that fails the outcome test, because it occupies a line and earns nothing.
