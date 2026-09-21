# Reconciliation — Beinecke MS 571, ff. 65r–69v

## Pilot sides (66v, 67r, 68r): Claude reader × google/gemini-3.1-pro-preview

Method: both readings cleaned by `clean_for_compare.py` (notes, line numbers, deletions stripped; additions kept; line-end hyphens joined), aligned with `tools/transcription_benchmark.py` (`disagreement/*.txt|json`); every surviving site cut from the native image (`crop_lines.py`) and decided by the operator before any outside reading was consulted. P1 = Claude agent, P2 = Gemini 3.1 Pro.

## f. 67r (148 words; graphemic disagreement 11.5 %, CER 2.0 %)
| Line | P1 | P2 | Page | Decision |
|---|---|---|---|---|
| 01 | sententiam | sententia | bar over a | P1 |
| 01–02 | [[transgressum … inoboedientiam]] | [[trans gressis a primis]] [[parentibus nostris pro inoboedientia]] | struck through, legible; per-sign, bar | P1 (P2 saw the deletion, misread inside it) |
| 02–03 | misericorditer redemit | misericordie redemptio | `misericordit̄ re/demit;` | P1 — P2 invented a noun phrase |
| 09 | septiformis | septa formis | ti-ligature | P1 |
| 10 | cum | cui | `cū` | P1 |
| 14 | ne[[…]] | nei(?) | ne + erased letter | P1 |
| 16 | quam cum [[p…]] | qua cum | `quā cū` + erasure | P1 |
| 17 | suscipit | suspirat | clear | P1 — P2 substituted a plausible word |
| 18 | offert | affert | **ꝓfert = profert** (same sign as `ꝓcessit` l. 16) | **both wrong**; found on the operator's read |
| 19 | uictus | uestitus | clear | P1 — P2 substituted |
| 21 | ⟨V⟩(?)uigiliarum | uigiliarum | stain in margin | P2's form (no initial) |
| 04, 05, 09, 13 | in ara, non solum, postmodum | inara, nonsolum, post modum | — | word division only |

## f. 66v (≈ 160 words; 26.3 %, CER 10.6 %)
| Line | P1 | P2 | Decision |
|---|---|---|---|
| 01 | pro iustis | pulsis | P1 (pro-sign + iustis) |
| 01, 06, 22 | exorat / sollempnitatis / primum | exor- / sollempnitat- / primu- | P1 — P2 drops letters at the gutter edge |
| 05 | aduersitatis | aduersitatibus | P1 |
| 07 | \curemus summopere/ | \curent summopere/ | P1 (`curem'`) |
| 07 | post(?) | per | **open** → post⟨?⟩ |
| 09 | [[lacrimabiliter deprecemur]] | not marked as deleted | P1 — P2 missed a strike-through |
| 11 | glorificationem(?) | glorificatione | **open** → glorificationem⟨?⟩ |
| 11–12 | miracu-/l[[a]]\a/ in terris; Presto\le/mur … \consequi/ beneficia | miracu- \consequi/ / la martyris; Prestet | P1 — P2 hallucinated *martyris*, lost the interlinear *le*, misplaced *consequi* |
| 13–14 | obtineamus / de celis | obtineamus mul- / decelis | P1 — P2 read a smudge as letters |
| 15 | quae nobis | que nobis per | P1 |
| 17–18 | admixtus est(?) / inclitus | admixti / incliti | P1 for *inclitus* (us-sign); **open** → admixtus est⟨?⟩ |
| 18 gloss | aderaldus | aderaldi | page: `Aderald'` with suspension — recorded unexpanded in the notes; not in the text |
| 20 | interrogat | interroget | P1 |
| 21 | sapienti et | sapienti | P1 (& at the edge) |
| 24–25 | propri- / a mi-(?) | propri- / ⟨...⟩ | **open** → propri⟨…⟩⟨?⟩ |

## f. 68r (151 words; 11.3 %, CER 4.2 %)
| Line | P1 | P2 | Decision |
|---|---|---|---|
| 03 | ueterem | carne | P1 — P2 substituted |
| 04 | inpuditiciis(?) | impudicitiis | inpudicitiis (in- clear; c/t not decidable) |
| 05 | induamus | induamur | P1 (us-sign) |
| 08 | fatiem(?) | faciem | faciem (c/t) |
| 09 | prosternamus | prosternamus(?) | pro-sign with loop confirmed on a zoom |
| 10 | inter | in | P1 (`int̄`) |
| 11 | usque \nunc/ consolatus est | … de gladiis \+ nunc/ | P1 — the + stands after *usque*; P2 left it where the margin is |
| 13 | pun\i/it | puniit | P1 |
| 18 | est \donum(?)/ eique | est. eiusque | P1; P2 omitted the marginal addition and misread *eique*; **open** → donum⟨?⟩ |
| 21 | per{hole}mittat | p{hole}mittat | P1 |
| 22 | uitiorum | uirorum | P1 |
| 23 | uirtu{hole}tum frui | uti et {hole} eum frua⟨...⟩ | P1, confirmed on a 2× zoom (GPT-5.5's *perpetua* rejected) |

## Totals
Substantive sites 41 (67r 10, 66v 20, 68r 11): P1 right 35 · P2 right 1 (no initial V) · both wrong 1 (*profert*) · left open 4 (+ 1 open site both flagged, *donum*). No line omitted by either reader; no show-through text transcribed by either reader (P2 on 68r attempt 1 noted "id est domini" beyond the edge and correctly excluded it).

## Escalation (GPT-5.5, 5 crops, $0.76)
e1 *post*: agrees, uncertain — no gain. e4 *uirtutum*: answered *perpetua* — wrong. e5 *ne*: agrees, mentions *nec* — no gain. e2, e3: 6,000 reasoning tokens, **no output**. Verdict: not worth its price here.

## Remaining sides: two independent Claude readers

Pass 1 and Pass 2 = independent Claude agents on differently framed images (A: block + 4 strips; B: block + 3 strips + magnified binding-edge crops). Alignment: `disagreement/*.txt|json`. Every site below was cut from the native image (`crop_lines.py`, crops in the private image directory) and decided by the operator. $0 metered.

| Side | Words | Word disagreement (graph) | CER |
|---|---|---|---|
| 65r | 126 | 2.4 % | 0.4 % |
| 65v | 165 | 2.4 % | 0.4 % |
| 66r | ≈ 165 | 9.0 % | 2.3 % |
| 67v | 172 | 2.3 % | 1.1 % |
| 68v | 184 | 1.1 % | 0.2 % |
| 69r | ≈ 171 | 2.4 % | 0.3 % |
| 69v ll. 1–2 | 10 | 0 % | 0 % |

| Loc. | Pass 1 | Pass 2 | Decision |
|---|---|---|---|
| 65r.06 | conueni\a/tis | conuen\a/itis | same observation; printed conveni\a/tis⟨?⟩ |
| 65r.07 | adtentissime | actentissime | P2 (ct on the page) |
| 65v.08 | preclaram festam | preclarum festum | P1 (bars over both a's) |
| 65v.19 | inpo-nere | impo-nere | P1 |
| 65v.24 | omnia \a/ | omni\a/ | P2's representation; \vitia⟨?⟩/ open in both |
| 66r.01 | inquiserat(?) | inquisierit(?) | **open** → inquiserit⟨?⟩ |
| 66r.01 | a deo(?) | ad eorum(?) | **open** → a deo⟨?⟩ (`adō` with bar) |
| 66r.03–04 | diui-/na | dum / licet | P2 on a zoom (`dū` / `lic&`); kept ⟨?⟩ because the line start is rubbed |
| 66r.04 | facultas \est/ | facul\tas/ est | facultas est (the raised letters are the scribe's line-fitting) |
| 66r.07 | inimici | inimica | P2 |
| 66r.11 | modo | m\o/do | P2 |
| 66r.13 | perspicuis | perspicue | P1 |
| 66r.16 | nulla | nulla\que/ | small sign under the line; recorded in notes, not printed |
| 66r.24 | quippe | qui pro | **P2** — pro-sign; confirmed by the parallel *pro iustis* on 66v.01 |
| 67v.04 | quecumque | quodcumque | P2 (`qđcūq;`) |
| 67v.10 | deum | dominum | P1 (`dm̄`) |
| 67v.10 | \poscamus/ … eamus | \preoptamus/ … eam | gloss **open** → \po⟨…⟩camus⟨?⟩/; *eamus* P1 (us-sign) |
| 68v.19 | spiritum | spiritu | P2 (`spū`, no m) |
| 68v.24 | scire(?) | scir⟨…⟩ | scir⟨e⟩ |
| 69r.14 | tim\e/tur | timetur | P1 (raised e) |
| 69r.15 | que | quia | P2 (q + superscript a) |
| 69r.11 | a celorum | a celorum | both; page has *a*, sense needs *ad* → a (sic) |

22 sites: Pass 1 right 6, Pass 2 right 10, other/open 6. The binding-edge magnifications (framing B) account for most of Pass 2's wins. Joins between sides checked: 65r→65v *dei bona / et bene placens*; 66r→66v *ut resipiscant / a malo*; 67r→67v *invigilat / luxuriam*; 67v→68r *crucem / christi*; 68r→68v *frui / atque in ea delectari*; 68v→69r *scir⟨e⟩ / non valemus*; 69r→69v *semper est / mirabilis*. 65v→66r (*iniquitatis / inquiserit⟨?⟩ … perditum*) and 66v→67r (*propri⟨…⟩ / prevaricationis*) remain syntactically unclear — both at flagged words.
