# Product Manager Resume Builder

Builds an ATS-ready product manager resume from the ground up. It interviews you about your work, rewrites your bullets with metrics you can defend, picks the right layout, and tailors the result to each job description. For first product roles, career switchers, and Senior PMs alike.

It handles three kinds of candidate, which need different advice: people who already hold a PM title, people switching in from engineering, design, marketing, data, sales, support, ops, or consulting, and people starting out with little professional experience. A seven-year engineer and a final-year student both lack a PM title and need close to opposite resumes.

Everything it needs is built in. There are no companion skills to install.

Plain Markdown with standard frontmatter, so it runs in Claude Code, Claude Desktop, Codex, Cursor, and anything else that reads agent skills. There is also a single-file prompt for chat tools that do not support skills at all.

## How a session runs

Seven steps. It tells you where you are at each one, and nothing gets written until step 4.

| Step | What happens | What you do |
|---|---|---|
| 1 | Getting started | Say whether you have a resume, then brain dump what is not on it |
| 2 | Target lock | Name the roles, the market, and the kind of company |
| 3 | Excavation | Answer questions about your work, one role at a time |
| 4 | Bullets | Review before and after on every rewrite |
| 5 | Assembly | Choose a layout from five options |
| 6 | Tailoring | Paste a job description and get a match score |
| 7 | Audit | Get the failure list and the estimates you need to defend |

Step 1 forks. If you have a resume, it diagnoses it and asks what you have done since. If you do not, a five-pass protocol builds from nothing. The layout choice waits until step 5 on purpose, because which one wins depends on what the interview turns up.

## What it does

Seven phases, run in order. Writing does not start until Phase 3. Everything before that exists to make sure there is something worth writing.

| Phase | What happens |
|---|---|
| 0 · Intake | Diagnoses your draft bluntly. If you do not have one, a five-pass protocol builds from nothing |
| 1 · Target lock | Role, level, market, company type, PM archetype. A resume with no target is a resume for no one |
| 2 · Excavation | Interviews you role by role about the bullets hiding the most. This phase decides the quality of everything after it |
| 3 · Bullet rebuild | Before and after for every bullet, so you learn the pattern instead of just receiving output |
| 4 · Master resume | Builds a master you never send, plus five templates to choose from |
| 5 · Tailoring loop | Per application, always derived from the master. Match score, keyword work, honest gap handling |
| 6 · Audit | Checks every line and reports what failed instead of quietly fixing it |

## Rules it will not break

It never invents a number. If you do not have a metric, it runs an estimation protocol that lands on a figure you confirmed, then labels it so you know to defend it in the interview.

It never inflates ownership. Led, Drove, Partnered with, and Contributed to mean different things to an interviewer, and a Senior PM will catch the gap in ninety seconds.

It never changes a job title. Titles get verified in background checks, so it gives you an honest scope line under the real title instead.

Everything it produces is text only and one page: no photo, no graphics, no columns, no tables. That is what survives ATS parsing. The two-page exception exists but has to be offered and accepted, never taken quietly.

## Install

**Download (no terminal needed).** Download this repo as a ZIP, unzip it, and upload the `skills/product-manager-resume-builder` folder to your assistant. In claude.ai that is Settings, then Capabilities, then Skills.

**Copy the prompt (no install at all).** Open [`dist/prompt.md`](dist/prompt.md), copy the whole file, and paste it into any chat. Works in ChatGPT, Gemini, and anywhere else.

**CLI.**

```bash
npx skills add githrish/product-manager-resume-builder -g -y
```

**Clone.**

```bash
git clone https://github.com/githrish/product-manager-resume-builder.git
cp -r product-manager-resume-builder/skills/product-manager-resume-builder ~/.claude/skills/
```

Then restart your assistant and say what you want:

```
Help me rebuild my PM resume for a senior product role
I'm a support lead trying to break into product and I don't have a resume yet
Tailor my resume to this job description
```

## What is inside

```
skills/product-manager-resume-builder/
├── SKILL.md                # the contract, the phase flow, the audit
└── references/
    ├── from-scratch.md     # blank page protocol, story inventory, recall prompts
    ├── targeting.md        # PM archetypes, level calibration, company types
    ├── markets.md          # country conventions, one-page exception, text-only rule
    ├── transitions.md      # switching in from another function with real seniority
    ├── breaking-in.md      # early-career entry targets, transferable evidence map
    ├── bullets.md          # formula, ownership ladder, metrics, anti-patterns
    ├── templates.md        # five layouts, one-page cutting order, formatting spec
    └── jd-and-ats.md       # requirement classification, dealbreakers, parser checks
```

Reference files load only when a phase calls for them, so a session tailoring to a US posting never pulls Japanese conventions into context.

## What is in this repo, and what it does not do

Worth knowing before you install anything into your assistant.

The skill is **nine Markdown files and nothing else**. No executable code, no network calls, no telemetry, no credentials, no dependencies. It cannot read anything you do not paste into the conversation, and it cannot send your resume anywhere. Read every file before installing; that is the point of keeping it plain text.

The repo does contain two pieces of code, neither of which ships inside the skill:

- `scripts/build-prompt.py` concatenates the skill files into `dist/prompt.md`. It reads and writes only inside this repo.
- `.github/workflows/build-prompt.yml` runs that script on push and commits the result.

`dist/prompt.md` is generated. Do not edit it by hand; it is overwritten on every build.

## For contributors

`SKILL.md` and `references/` are the source of truth. `dist/prompt.md` is generated, so do not edit it by hand. After changing the skill, run:

```bash
python3 scripts/build-prompt.py
```

A GitHub Action does the same on every push to `main` that touches `skills/`, and commits the result.

## Getting the most out of it

Spend fifteen minutes on a brain dump first. List everything you did in each role: what you shipped, decisions you made, fires you put out, people you convinced, things that failed. Do not write bullets and do not edit. Phase 2 is designed to mine exactly this.

When it asks you questions, answer with stories rather than summaries. "We were losing merchants at onboarding and nobody knew why, so I sat in on twenty calls" gives it far more to work with than "improved onboarding."

## License

MIT
