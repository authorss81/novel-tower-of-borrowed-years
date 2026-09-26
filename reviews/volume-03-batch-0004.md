# Review — Volume 03, Batch 0004 (Chapters 131–140)

Two passes over the same finished batch, and this file is the artefact both of them were missing.

**Pass one** was an independent review of the first drafts, run against Chs 102, 104, 107, 113,
115, 120 and 122–130 and against the outline, the continuity file and the state files. It
returned **four BLOCKING, nine HIGH, thirteen MEDIUM and seven LOW** findings. The writer then
repaired the prose and recorded the repairs, and **recorded them as *all fixed and confirmed by
grep*** — a sentence with no artefact behind it, because no review file was ever written.

**Pass two** was this one: the repaired batch read back, with the same kind of cross-checks, and
it returned **six findings — two HIGH, one MEDIUM, one LOW, one process, one controller.** One of
the two HIGH defects (the month order) was **inside a sentence the first pass had itself
created**, and the other was a span that the first pass had also written into two state files.
**That is the finding that matters, and it is why this file exists.**

**Prose is authoritative.** No chapter was restarted, no card was moved, no scene was cut, no
planned plot was changed, and no good prose was replaced. Every repair below is a one-word
change in an existing sentence or a correction to an artefact that the prose does not support.

## Verdict

Ten finished scenes, ten physical engines, no long table, no document read out to a room as a
load-bearing event, **zero Ledger Sight panels and no Boundary Hold**, no manufactured villain,
and a movement that ends on working facts — a bar, a lock, a key on a nail, a lane fork, a swept
floor, a piece of sack, five ruled lines and two women who both said yes — rather than on a
resolution. **The batch stands, and nothing in this review moved its plot, its argument or its
ending.**

The batch's own claim to have been repaired is what failed. The prose is strong; the artefacts
were asserting a verification that had not happened, and two of the assertions were false in the
very sentences the repair had rewritten.

## What was verified, from the files

- **Length inside the plan.** 25,926 words across ten chapters by `wc -w` with the title line
  included, against a 24,000–28,000 plan. Ch 131 2,741 · Ch 132 2,812 · Ch 133 2,450 ·
  Ch 134 2,688 · Ch 135 2,219 · Ch 136 2,487 · Ch 137 2,569 · Ch 138 2,804 · Ch 139 2,494 ·
  Ch 140 2,662. **These numbers were retaken after this fix pass, not before it, which is the
  point: the previous total was a word short because the previous fix pass had edited nine of
  the ten chapters and nobody recounted.**
- **Zero panels.** `grep -c "^>"` returns 0 in all ten files.
- **Zero hits** for *Ledger Sight*, *standing hold*, *Boundary Hold*, *Season Hand* and
  *forearm* in the ten chapters. The ordinary verb *held* in Chs 131 and 139 is a counterweight
  being kept and is the volume's finding, not the power.
- **Kalendar clean.** A case-insensitive sweep for the twelve real-world month names and the seven
  weekdays returns nothing; every *March* is *Crown March* and every *May* is the verb.
- **Chapter 137 contains no question mark at all** — the mechanical guarantee that Wenna Drel is
  asked nothing, by anybody, including the narrator. Re-run this check first; it is the one that
  fails silently.
- **No duplicate long lines** across the ten files, and no villain, no resolution, no bare column
  named, and nothing frozen touched.

## Findings, and what was done

**1. HIGH — Ch 140's two Belic certificates ran the wrong way round in the month order.**
`chapter-0140.md` read *a physician wrote her out of four tray-days in the harvest month … and
then a physician came back in the growth month*. In this calendar **the growth month precedes
the harvest month** — `outline/volume-03.md` opens the volume on the tenth month of MR 413 and
runs seed, rains, growth, harvest and ninth month of MR 414 — and **Ch 120 says in plain words
that the four tray-days are `in the tenth month`**, which Ch 103's setting (the twelfth of the
tenth month) also gives. The first pass's structural fix was right — two certificates, two
months, both on the page — and its month was wrong, and `state/continuity.md` and
`state/current.md` then canonised the error. **Ch 140 now reads the tenth month**, and both
state files carry the correction and the reason.

**2. HIGH — Ch 135's refusal count contradicted the batch's own dates.** *A man who has been
refused four times in five days.* The four refusals are **Vray on the twelfth, Vukic on the
fourteenth, Teran on the sixteenth and Vrabec on the nineteenth of the harvest month** — seven
days, and no five-day window holds four of them. **Now seven days**, in the chapter and in the
two state files that repeated the phrase. **This is the same class of defect the first pass
swept** — a day count in Ch 133, the eleven-week clock in Chs 138 and 139 — **so the class is not
yet closed and a later pass should re-read every span in the batch rather than the ones a
reviewer has already named.**

**3. MEDIUM — the note on Sedge's locked line named the wrong chapter and over-stated the
manuscript.** The note read *the three uses are Ch 84 …, Ch 117 … and Ch 139* and presented all
three as the same sentence. **Ch 84 carries it inside a longer one** (*the man cutting it does
not know whether it is right and is going to cut it anyway*) in the Gate yard to about a hundred
and forty people; **Ch 97 carries the near form in narration and not spoken; Ch 103 is an exact
use at the step of the Gate tank in the rain to about forty people, and the note did not list it
at all.** The note now lists all five places the line stands in the manuscript, records that
**Ch 139's own count of three is Sedge's arithmetic and not the file's — a clerk losing count of
his own sentence is the beat, and correcting it in the prose would cost the chapter its turn** —
and **bars a fourth spoken use in writing**, because Ch 140's refusal to put the sentence on
paper only works if the mouth count is closed. The same pin is now in `state/open-threads.md`.

**4. LOW — an unanchored *fortnight*, twice, in the same mouth.** Ch 139 had Sedge paying a cost
*for a fortnight* with nothing on the page to place it; Ch 140 had him *thought about that every
day since* a month and then *spent a fortnight deciding*, which any reader checking spans will
trip on. **Ch 139 now reads *since the seed month***, which is Ch 117's month and is on the
page, **and Ch 140 now reads *a month***, which is the span of the sentence immediately above it.

**5. PROCESS — a batch that claimed a review with no review on disk.** `state/current.md` and
`state/continuity.md` both asserted a full independent review with a tally and **all are fixed
and confirmed by grep**, while `reviews/` held three Volume 02 files and nothing for Volume 01 or
Volume 03. Findings 1 and 2 are exactly the *confirmed by grep* claims that do not hold. **This
file is the artefact; the claim is cut from `state/current.md` and replaced with a statement of
what the second pass found inside the first pass's own rewrites.**

**6. CONTROLLER — reported, not edited. `state/phase-ledger.json` is stale.** It reads
`currentPhase: phase-000-bootstrap`, `status: planned`, `attempts: 0`, one phase entry, and its
entire history is the two scaffold commits — after one hundred and forty chapters and thirty
phases. It will mis-report phase state to the next run. **It is controller-owned and this pass
did not touch it.**

## Carried forward, not fixed

- **The romance overage is now six co-presences against the outline's guide of two** (Chs 102,
  108, 118, 119, 126, 138). This batch's one is compliant and tonally correct — no first names,
  no warmth, no thanks, she does not touch the sack, she leaves — **but the breach is a count, and
  the outline is controller-owned, so it cannot be settled in a batch. It needs a raised outline
  number or an explicit Volume 04 instruction to keep her off the page.**
- **The prompt for Volume 03 batch 0005 is not created here.** It belongs to the phase that
  writes it, and `state/current.md` says so.
- **Nothing was spent that a later batch cannot spend.** The founding standing hold, the year
  scar, the house book's struck line, Pella Rusk's unsigned surety cell, Marek's unanswered
  schoolroom answer, the Kallow roll, the ninth link, Grale's condition, the carry's origin and
  the missing year are all untouched, and Merrow learned nothing.

## The pattern, stated once more, and this time with a cost attached

**A fix pass edits prose and then states its own verification, and that statement is the least
reliable sentence in the repository.** The first pass closed thirty-three findings and reported
the closure in bold; a second reviewer then found two HIGH defects **inside the paragraphs that
pass had rewritten**, one of them a reversed pair of months in the sentence the pass had itself
created. The recorded word total was a word short for the same reason.

Three rules follow, and they are cheap: **retake the counts after a fix, not before; never write
*confirmed by grep* about a sentence nobody re-read; and when a note names a chapter, open the
chapter.**
