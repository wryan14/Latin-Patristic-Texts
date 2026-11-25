# Reconciliation — Houghton MS Lat 184, ff. 1r–16v (2026-11-24)

Pass 1 = `reading_A/` (4 Claude agents, half-page crops, pre-standard notation). Pass 2 = `pass2/` (4 fresh Claude agents, blind to Pass 1, page + 3 strips, READER_INSTRUCTIONS.md). Line-aligned differences: `compare_passes.py` → `disagreement/` (154 differing line pairs of 768; mean key CER 1.8 % incl. notation). Reconciliation: 4 Claude agents, RECONCILER_INSTRUCTIONS.md, every disagreement and every flagged word cropped from the 2400 px image and decided; logs `reconciled/<page>.log.json`, crops in the private image directory (`tmp/rec_*`). $0 metered. Stage reached: **reconciled** (curator check not done).

Decisions: 328 (P2 146, P1 62, both 46 [agreed but checked], neither 31 [both passes wrong], open 11, notation 32).
Result: 6,183 words; 84 words still `(?)` (1.4 %), 1 illegible spot.

Cross-page conventions fixed by the operator:
- q + stroke through descender, no superscript = **quia(?)** (never spelled out on these pages; quod = qd, quam = q+a, qui = q+i).
- the same sign + superscript hook = **quoque(?)** (alternatives quidem/quasi) — all four reconcilers independently.
- bare "v." preceded by a point (f.12v ll.13, 24; f.13 ll.13–14; f.16 l.20) = **uidelicet(?)**, alternative explanatory uel; the scribe writes disjunctive vel as ł (f.13 l.22). All contexts explanatory → English "that is".
- closing formula "Qd ipse p(st)" = Quod ipse prestet(?); suspended formulas otherwise kept as letters unless written out elsewhere.

Key readings confirmed: f.10 ll.9–10 *Uidemus romanum imperium destrui. De inde et leges humane penitus defecerunt.*; f.12 l.11 *Et ideo dicitur uulgo communis ebdomada*; f.12 l.2 rubric *Sermo in ebdomada que dicitur communi(s)* (rubric ꝯmi, margin guide ꝯmunis); f.2/2v *Unde pariter* (no break); f.9 *per hoc* ×3 and *pro his*; *Zacheus*.

Page joins: breaks at **f.1v→f.2** (Lent sermon ends "et sic tu"; Pentecost sermon acephalous → leaf lost), **f.4v→f.5** (f.5 opens with a free-standing blessing "Modo committo corpus et animam uestram…" after a closed formula — loss or detached formula, undecidable), **f.16v→f.17** (2nd dedication sermon breaks off "Et quidam(?)"; f.17 begins section 2). f.1r is acephalous (first leaf lost). All other joins hold (f.3v→f.4 hangs on "ei commisit(?)").
