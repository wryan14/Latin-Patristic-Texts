# Stage 1 reconciliation log — HAB Cod. Guelf. 602 Helmst., ff. 2v–3v and 16v–17v (Phase 9B, 2026-09-14)

Method (MANUSCRIPT_TRANSCRIPTION_STANDARD.md §7): Pass 1 = the Phase 9A sizing drafts (general-purpose Claude agents, one per text, reading the HAB 2000 px images in strips), split per folio (`pass1/`). Pass 2 = six fresh general-purpose Claude agents, one per folio, forbidden to search or read any file other than the crops (`pass2/`). Alignment: `tools/transcription_benchmark.py` (graphemic layer). Every disagreement was re-cut at line level (`crop_line.py`) and decided on the image by the operator (Claude Fable 5.1 session) before any parallel or edition was consulted; no third reading was needed (disagreement per page 1.9–7.1 %, threshold 10 %). No metered call.

| Page | Words | Disagreement (graph) | Sites | P1 right | P2 right | both wrong | uncertain after inspection |
|---|---|---|---|---|---|---|---|
| 2v | 172 | 3.5 % | 5 | 3 | 2 | 0 | 0 |
| 3r | 178 | 5.6 % | 7 | 1 | 3 | 0 | 3 |
| 3v | 158 | 4.4 % | 6 | 3 | 2 | 0 | 1 |
| 16v | 207 | 1.9 % | 4 | 0 | 2 | 1 (*parvitas*) | 2 (incl. *parvitas*) |
| 17r | 227 | 7.1 % | 12 | 6 | 5 | 0 | 4 |
| 17v | 159 (sermon part) | ≈ 5 % | 7 | 4 | 3 | 0 | 3 |
| **all** | **1,101** | — | **41** | **17** | **17** | **1** | **18 flagged ⟨?⟩ in the reading text** (13 from disputed sites, 5 carried from both passes) |

## Verdicts

| Site | Pass 1 | Pass 2 | Page shows | Decision |
|---|---|---|---|---|
| 2v.01 | uiuentium(?) | inuenientium | `uiuẽtium` | **viventium** |
| 2v.02–03 | esurie-tium | esurientium | `eſuriẽ-tium`, bar | **esurientium** (P2) |
| 2v.03 | Bernardi(?) | bernardus | `Bñi.` — source tag, genitive | **Bernardi** (P1) |
| 2v.07 | preminentie | preeminentie | `p̄eminentie` (p̄ = pre) | **preeminentie** (P2) |
| 2v.12–13 | In inimi-corum | imicorum | `In inimi-|coꝝ` | **in inimicorum** (P1) |
| 2v.28–3r.01 | diui- / na | diuin | `diui-` at line end, `na` on 3r.01 | **divina** (page join) |
| 3r.05 | conuescendum(?) | conuersandum | `cõueſ?ndũ` — s/rs ambiguous | **conversandum⟨?⟩** (alternative *convescendum*) |
| 3r.08–09 | commen-dandum | comdandum | `cõm-|dandũ` | **commendandum** (P1) |
| 3r.10 | a minime(?) | in munimine(?) | `ĩ munimẽ actõis` — minims; a sign before `ĩ` may be *et* | **et in munimen⟨?⟩** (operator full read: Tironian *et* precedes `ĩ munimẽ`; alternatives *in munimine*, *a minime*) |
| 3r.17 | incerte(?) | in certe(?) | `incerte` written without a break | **incerte⟨?⟩** (sense unclear; *interne* not supported by the letters) |
| 3r.20 | in permixtione(?) | impermixtionem | `in p̄mixtionẽ` — two words, final bar | **in permixtionem** |
| 3r.20–21 | augmen-tationem | aucmen-tationem | `aucmẽ-` (scribe writes c) | **aucmentationem** (page spelling) |
| 3r.26 | super | sibi | `ſĩ` | **sibi** (P2) |
| 3v.02 | profectiuum | perfectiuum | `ꝑfectiuũ` (per-sign) | **perfectivum** (P2) |
| 3v.06 | angelice pronunciationis | anglice prenunciationis | `anglice p̄nũciatõis` | **anglice prenunciationis** (P2; *anglice* is the page's spelling of *angelice*) |
| 3v.08 | periurii | yuurij | `ꝑiurij` (per-sign + iurii) | **periurii** (P1) |
| 3v.09 | beatificandi | beneficandi | `bt̃ificãdi` | **beatificandi** (P1) |
| 3v.13 | confusione | conuersione | `cõu?ſione` — f/u ambiguous | **conversione⟨?⟩** (alternative *confusione*) |
| 3v.22 | dominum | deum | `dñm` | **dominum** (P1) |
| 16v.16 | distinguuntur | distinguntur | `diſtingunt'` | **distinguntur** (page spelling) |
| 16v.18 | (note) maioribus | maioribus | `minoribꝫ` with superscript *ai* and two subpunction dots under *in* | **maioribus** (scribal correction of *minoribus*) |
| 16v.19 | puritas(?) | prouicias | `p̄uitas` — p with bar = *par* | **parvitas⟨?⟩** (both readers wrong; fits the triad parvitas / conformitas / prudentia) |
| 16v.22 | eorumdem; imitabiles(?) | eorundem | `eoꝝdem`; `imitabiles` minims | **eorundem**; **imitabiles⟨?⟩** |
| 17r.01 | primus | prius | `pri⁹` | **prius** (P2) |
| 17r.02 | \<per\> | (per) | interlinear `per` above the line | **\per/** (scribal addition, both) |
| 17r.03 | apostolica(?) | a propheta | `a pph̃a` before the Ps. 44 quotation | **a propheta⟨?⟩** (P2) |
| 17r.06 | pulchra | pulchritudine | `pulc̃` + superscript = *pulchra* | **pulchra** (P1) |
| 17r.07 | attende | adtende | `adtende` | **adtende** (page spelling) |
| 17r.08 | spem | spem | `ſpẽ` — the same compendium read *Specie* in 17r.03 | **spem (sic)** (operator full read: written out `ſpem`, not abbreviated; the sense wants *speciem*) |
| 17r.12 | quasi(?) prepropere(?) | quam prepropere | `q̃` ambiguous; `pre-ppere` | **quasi⟨?⟩ prepropere⟨?⟩** |
| 17r.15 | iuribus | uiribus | `uiribꝫ` | **viribus** (P2) |
| 17r.16 | premetiens(?). quod | que | `p̄metiẽs`; `q̄` | **premetiens⟨?⟩ quod⟨?⟩** |
| 17r.18 | pharisaica re-prehensione | pharisayca rephensione | `pharisayca re-|p̄hensione` | **pharisayca reprehensione** (spelling P2, expansion P1) |
| 17r.19–20 | im-ponentes | inponentes | `in-|ponẽtes` | **inponentes** (page spelling) |
| 17r.22 | Enimvero | cum uero | red-touched `E` + `nĩ uero` | **Enimvero** (P1) |
| 17r.24–25 | amite(?) dicendi. cedere(?) scorpionibus | cetere sermonibus | `amite dicendi. cede͛` / `ſcorpionibꝫ cõſueũt` | **amite⟨?⟩ dicendi cedere scorpionibus consueverunt** (3 Reg. 12:11; *amite* unresolved) |
| 17r.28 | precipiant | percipiant | `p̄cipiant` | **precipiant** (P1) |
| 17v.01 | quod | que | `q̄` | **quod** |
| 17v.05 | quam; tressis(?) | quoniam | `q̃m`; `treſſis` | **quam⟨?⟩**; **tressis⟨?⟩** (Persius 5.76 *non tressis agaso*) |
| 17v.06 | aselli | asselli | `aſſelli` | **asselli** (page spelling) |
| 17v.07 | soletur(?) | solet | `ſolet̃` with a suspension | **soletur⟨?⟩** |
| 17v.08 | quia(?) | quod | `qꝫ` — a sign this hand also uses for *quod* (17v.14 *quod petrus audivit*) | **quia⟨?⟩** (causal sense with *Ideo*; *quod* possible) |
| 17v.09 | amiciciam | amicicia | `amiciciã` | **amiciciam** (P1) |
| 17v.16 | immarcessibiliter(?) coronatur | inmarcessibiliter coronatus | `ĩmarceſſibilit' coronat⁹` | **inmarcessibiliter coronatus** (P2) |

Sites both readers agreed on that are nonetheless flagged in the reading text (uncertain expansions carried from both passes and confirmed as unresolved on the image): 2v.23 *incelabile*, 3r.07 *affandum*, 17r.24 *amite*, 16v.22 *imitabiles*, 17v.05 *tressis*. Text boundaries confirmed on the images: text A 2v.01 (rubric ›De deo‹, red capital) to 3v.27 *impetrat* with red line-fillers, rubric ›Incipit Regula Basilii‹ on 3v.28; text B 16v.10 (red initial C; the rubric stands at the end of that line after the first clause) to 17v.19 *amen*, rubric ›Bernardus‹ on 17v.20. Two page joins inside the texts (*divi-|na* 2v/3r; *solli-|citus* 16v/17r; *idipsum | precipiant* 17r/17v) verified; no line omitted (28 + 28 + 27 and 19 + 28 + 19 lines accounted for). Lesser's explicit *postulata imperat* is read by both passes as *impetrat* (`impetrat` with a t): the page reading stands.
