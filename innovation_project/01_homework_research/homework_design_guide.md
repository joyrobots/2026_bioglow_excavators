# JoyRobots Excavators — Homework Design Guide

Every weekly homework sheet follows this guide so the kids see the same layout each week and spend their energy on the answers, not on figuring out the page. Week 9 (`homework_week09.html`) is the reference sheet. Copy it to start a new week.

## 1. Files and naming

| What | Where |
| --- | --- |
| Source | `innovation_project/01_homework_research/homework_weekNN.html` |
| Printable | `innovation_project/01_homework_research/homework_weekNN.pdf` |
| Per-kid variants (only when needed) | `homework_weekNN_<firstname>_<topic>.pdf` (lowercase, as in week 8) |
| In-class worksheets | `innovation_project/01_homework_research/In_class_worksheets/` |

Always commit both the `.html` and the `.pdf`. Never push without asking Kirby.

## 2. Who it is for

Kids aged 6 to 12. The youngest are still learning to write, and all of them lose focus fast, so:

- **Big writing space.** Ruled lines about 40 px tall (roughly 14 mm), number boxes about 44 × 32 px, numbered step lines 40 px. Four lines per open question, no more. Kids read empty lines as a to-do list, so many lines feels like an essay. A 6-year-old writes large; cramped lines get skipped.
- **One or two pages.** One part per page when two are needed. Never let a stray line or box spill onto a page by itself.
- **5–7 questions max.** If it needs more, it is two weeks of homework.
- **Short sentences, everyday words.** Say "points" not "scoring criteria". Say "tool that goes on the robot" next to "attachment".
- **Every question gets a "Hint:" line** in italics underneath. The hint lists 2–3 concrete things to remember, phrased as questions.
- **Blanks, not paragraphs.** Ruled lines (four per open question), tick boxes, number boxes, or short fill-ins. Build fill-ins with bordered `.blank` spans, never typed underscores on top of a ruled line (it prints as a doubled line). Use bulleted lines (not numbered) when the answer is a sequence, so nobody feels they must fill every one. Say "You don't have to fill every line" in the intro.
- **Use real team facts** when you have them: mission numbers, the Stouffville Road tunnel, TRCA, Dr. Ruppert, the sandbox model. Real examples beat generic prompts.

## 3. Page structure (top to bottom)

1. **Brand line** — small caps, grey: `JOYROBOTS EXCAVATORS | TEAM #65536 | WEEK NN HOMEWORK`
2. **Title** — green, 3–6 words, kid-facing. "My Mission and My Attachment", not "Robot Design Rubric Prep".
3. **Subtitle** — one grey line saying what it is for. "Get ready for our Robot Design explanation to the judges."
4. **Name / Date** line.
5. **Intro box** — pale green, green left border, max two lines. State the real-world reason (what the judge or expert will ask) and how to answer ("short answers, in your own words, with real examples").
6. **Part headings** — "Part 1 — <kid-facing name>" with a small grey tag giving the official term, e.g. `Judges call this "mission strategy"`. One or two parts per sheet.
7. **Questions** — numbered across the whole sheet (1–6), bold question, italic hint, then the answer space.
8. **No closing box.** The sheet ends after the last question. Reminders go in the session slides, not on the sheet.

## 4. Tie each sheet to a rubric row

Each sheet should target one or two rows of the official FLL rubric and say so in the part heading tag. Robot Design rows:

| Row | What the judges want to hear |
| --- | --- |
| Identify | Which missions we chose and why (mission strategy); what resources or help we used |
| Design | Everyone contributed ideas; everyone has building and coding skills |
| Create | Clear explanation of attachments and their purpose; code and sensor use |
| Iterate | Repeated testing; improvements that came from testing |
| Communicate | Process and lessons learned; pride and enthusiasm |

Innovation Project rows use the same five names. Rubric source: https://firstinspires.blob.core.windows.net/fll/challenge/2025-26/fll-challenge-unearthed-rubrics-color.pdf

## 5. Visual style (copy the CSS from `homework_week09.html`)

| Token | Value |
| --- | --- |
| Page | Letter, margins 12 mm top, 15 mm sides, 10 mm bottom |
| Font | Helvetica Neue / Arial, 11 pt body, line-height 1.3 |
| Ink | `#1a1a1a` |
| Accent green | `#1f6f3f` (title, part headings, step numbers, box border) |
| Soft green | `#e8f3ec` (intro box, finish box) |
| Rule grey | `#9aa3ab` (answer lines, boxes) |
| Muted text | `#555` (brand line, subtitle, hints) |
| Answer line | 1 px grey bottom border, 40 px tall |
| Tick box | 12 px square, 1.5 px ink border, 2 px radius |
| Option cards | Equal-width flex boxes, 1.5 px grey border, 6 px radius, bold label + one-line definition, optional "How many:" blank pinned to the bottom |

Keep it black-and-green only. No clip art, no emoji in the body (the older week 4 sheet used them; week 7 onward does not).

## 6. Render and check

```bash
cd "innovation_project/01_homework_research"
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --disable-gpu \
  --no-pdf-header-footer --print-to-pdf="$PWD/homework_weekNN.pdf" "file://$PWD/homework_weekNN.html"
```

Then confirm the page count and look at a preview image before handing it over. If it spills to a second page by a few lines, either tighten spacing (box padding, intro length) or split one part per page with a `page-break-before`. Do not shrink the writing lines below 34 px to make it fit.

## 7. Checklist before it goes out

- [ ] One or two full pages, one part per page, nothing orphaned
- [ ] 5–7 questions, each with a "Hint:" line
- [ ] Part heading names the rubric row it feeds
- [ ] Kid-facing words; official terms only in the grey tags
- [ ] Enough lines or numbered steps that no answer feels capped
- [ ] No typed underscores; all blanks are bordered spans or ruled lines
- [ ] `.html` and `.pdf` both saved with the `homework_weekNN` name
