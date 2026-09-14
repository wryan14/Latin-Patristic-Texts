# Stage 1 transcription QA — HAB Cod. Guelf. 602 Helmst., texts A and B (Phase 9B, 2026-09-14)

Scope: the two reading texts in `final/` (text A `ms-hab-602-helmst-p1-002`, ff. 2v–3v, 509 words; text B `ms-hab-602-helmst-p1-004`, ff. 16v–17v, 513 words), their provenance files and the pipeline `source.txt` derived from them. Standard: `MANUSCRIPT_TRANSCRIPTION_STANDARD.md` v1.0 (D043). No metered call.

| Check | Method | Result |
|---|---|---|
| Provenance validates | `tools/validate_transcription_provenance.py --strict` on both files | OK / OK (D036 fields, verification record, image rights, textual unit) |
| Independent second reading | six fresh agents, one per folio, no access to Pass 1 or any edition (`pass2/`) | done; disagreement 1.9–7.1 % per page, all below the 10 % third-reading threshold |
| Every disagreement inspected | 41 sites re-cut at line level and decided on the image (`RECONCILIATION.md`) | 41 / 41 |
| Unresolved readings | listed with alternatives in `known_uncertainties` and flagged `⟨?⟩` in the text | A: 6 flags; B: 12 flags (18 words of 1,022 = 1.8 %) |
| Abbreviation expansions | every disputed expansion checked against the sign (bars, per/pre/pro, -us, -que, q̃/q̄, suspensions); the scribe's own full spellings followed | 15 expansion disputes resolved; the flagged ones remain flagged |
| Minim confusions | disputed minim strings inspected (viventium, inimicorum, munimen, incerte, conversione, parvitas, imitabiles, viribus) | resolved except the four flagged |
| Word boundaries | in permixtionem / incerte / a propheta / in munimen checked on the page | recorded; modern word division applied (standard §5.1) |
| Folio joins | 2v→3r *divi-na*, 3r→3v *protectionem. / orationis*, 16v→17r *solli-citus*, 17r→17v *idipsum / precipiant* | all four verified on both images; `[f. Nr]` marks placed at the join |
| Possible omissions | line counts per page (28/28/27 and 19/28/19) against the reconciled files; no line unaccounted; both passes have equal word counts per page (±2) | none found |
| Text boundaries | 2v.01 rubric ›De deo‹ + red capital → 3v.27 *impetrat* + line-fillers, rubric ›Incipit Regula Basilii‹ 3v.28; 16v.10 red initial C + rubric ›Sermo magistri Gerhardi‹ → 17v.19 *amen*, rubric ›Bernardus‹ 17v.20 | confirmed on the images; matches Lesser except *impetrat* for his *imperat* |
| Operator full re-read | every strip of all six pages read against the reconciled lines after reconciliation | done; two refinements found (3r.10 *et in munimen*, 17r.08 *spem* written out) and applied |
| Nothing normalized toward a parallel | no edition or parallel consulted before adjudication; Bernard SCC 15.6 recognised only as the source tag *Bernardi* | confirmed |
| Nothing reconstructed | the defective-looking opening of text B (*Cuius …*) is transcribed as written; no supplement | confirmed |
| Derived `source.txt` | flags, ¶, rubric brackets and `\…/` stripped; `[f. Nr]` kept; one heading line per text | 8,427 chars, 6 folio markers, 2 headings |

## Review status claimed

`verification.stage = reconciled`, `review_status = fully-reviewed`, `uncertain_passages_present = true`. **Not** `curator-verified`: the standard's curator check (§7) was performed as a full re-read by the operator (the Claude session), and the provenance records it as such, but the human curator has not signed the version. The sign-off is requested at the Stage 1 editorial gate; if given, the stage becomes `curator-verified` (version 1.0 unchanged, `curator_check.by` updated). Recommendation for the standard v1.1: name the two checks separately (operator full read; curator sign-off).

## Known limits stated for publication

- 18 flagged words (1.8 %); the Phase 9A calibration on the same hand predicts about 0.5 % of words (≈ 5) may be shared misreadings invisible to double reading. Both figures go into the edition's provenance note.
- The scribe's spellings are kept (anglice, aucmentationem, adtende, inponentes, asselli, pharisayca, distinguntur, spem); the translation reads them by sense and records the reading in its notes.
- Lesser's explicit *postulata imperat* vs the page's *impetrat*: the page governs.
