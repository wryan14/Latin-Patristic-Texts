# Latin Patristic Texts — the open corpus of Bibliothecarius Modernus

This repository is the cloneable text corpus of [Bibliothecarius Modernus](https://bibliothecarius-modernus.github.io), an independent digital library of neglected Latin literature, publishing complete open translations, parallel texts, contextual research, audio and video editions, and machine-readable scholarly data — and, where the sources require it, new transcriptions from manuscripts.

For each published edition the corpus holds the public-domain Latin source as used, the complete English translation, and the edition's `translation.json` (Latin and English segment by segment, with method, provenance, review status and rights). The corpus is a core destination of every edition and stays where it is: the directory structure below is stable, and links into it from the website, YouTube descriptions, Archive.org items and Zenodo records are kept working.

## What the repository contains

```
Patrologia_Latina/
├── README.md                             # human-readable works catalog, by author
├── CATALOG_INDEX.csv                     # directory ↔ catalog id ↔ website / YouTube / Archive / DOI (generated)
└── vol_XXX/                              # Patrologia Latina volume
    └── Author Name - English Title/
        ├── Latin/
        │   ├── *.txt                     # the Latin source text as used (public domain)
        │   └── transcription_provenance.json   # only for Bibliothecarius manuscript transcriptions (see below)
        ├── Author-Name-English-Title-Full-Text-Edition.txt   # the complete English translation
        ├── translation.json              # parallel text + metadata (2025–26 editions; per-segment provenance from 2026)
        ├── SSML/                         # narration markup (production artifact, where present)
        └── Subtitles/                    # subtitle track (production artifact, where present)
Libri_Carolini/                           # legacy layout (2024): the Libri Carolini, kept in place
Vita_Annonis_Minor/                       # legacy layout (2024): kept in place
youtube_videos_export.csv                 # export of the channel's video list (2025)
```

### Latin source vs Bibliothecarius contribution

- **Latin source text** — J.-P. Migne, *Patrologia Latina* (1844–65), reproduced as extracted for the parallel translation; public domain. No rights are claimed over the Latin. The underlying digitised database is not redistributed here; the corpus holds only the Latin paired with a published translation. Where a `translation.json` records a `source_kind`, the values are `migne-pl` (the default), `printed-edition`, `bibliothecarius-transcription` and `third-party-ocr-htr`.
- **Bibliothecarius contribution** — the English translation, the full-text edition, `translation.json` metadata, notes and chapter titles, subtitles, SSML, and any Latin transcription or markup the library itself made. All of it is dedicated to the public domain under **CC0 1.0** (see [Rights](#rights)).

### Provenance and review status

Editions made since September 2026 (the library's "v2" workflow) carry, inside `translation.json`, per-segment model provenance (`metadata.provenance`: the translation model, provider, output contract and per-call usage), the recorded corrections (`metadata.corrections`: original, corrected text, the Latin basis, the reason, the reviewing model and the curator's judgement), the rights statement (`metadata.rights`), the catalog id and the source location (`metadata.catalog_id`, `pl_volume`, `col_start`, `col_end`). They passed a deterministic source-coverage check and an independent review by a model of a different family before publication, and their review status is published in the [machine-readable catalog](https://bibliothecarius-modernus.github.io/api/README.md) (`coverage-verified`, `human-reviewed`, `spot-checked`, `defect-recorded`, `unreviewed`). A review status says what was checked; it is not a guarantee of fidelity.

**Legacy corpus caveat (2024–2025).** Most of the works here were produced before that workflow, with earlier models and lighter checks: no segment-level coverage check, no independent review, no per-segment provenance, and `translation.json` only for the later ones. They are preserved as published (review status `unreviewed`), repaired individually when a real defect is found, and never presented as more than they are. Twelve editions are known to be missing a contiguous stretch of their Latin source; they are flagged `defect-recorded` in the catalog with the extent of the gap, so that a citing reader or program does not assume completeness. Directory names and older file layouts are kept as they are.

### Catalog ids and citation

Every edition has a stable catalog id, `plNNN-SSS` (Patrologia Latina volume and sequence). `Patrologia_Latina/CATALOG_INDEX.csv` maps each directory to its catalog id, publication record, PL location, review status, translation model and public URLs; the same facts are in `https://bibliothecarius-modernus.github.io/api/catalog.json` (schema `bibliothecarius.catalog/1`). Segments of the 2026 editions can be cited by passage locator, `plNNN-SSS[/part]:cNNNN[a-d]:chunk-n` (catalog id, PL column, segment number = the `chunk_id` in `translation.json` and the `#chunk-n` anchor on the edition page). Historical works have no chunk-to-column mapping; do not infer column precision that is not stated.

Cite a work as: *Author, Latin title. Bibliothecarius Modernus edition, year, catalog id plNNN-SSS; passage locator or URL.* Each edition page offers BibTeX/RIS; `CITATION.cff` describes the corpus as a whole.

## Rights

Owner decision (Bibliothecarius Modernus v2, D031, 2026-09-13), stated the same way on the website, on Archive.org and in every new `translation.json`:

- **Latin texts** (`Latin/*.txt`, `source.txt`, the Latin fields of `translation.json`): public-domain source material — J.-P. Migne, *Patrologia Latina* (1844–65), or the named manuscript — reproduced as extracted for the parallel translation. No rights are claimed over the Latin; the underlying digitised database is not redistributed here.
- **Everything Bibliothecarius Modernus created** — the English translations, full-text editions, `translation.json` metadata and notes, subtitles, SSML, transcriptions and every other scholarly contribution in this repository: **[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)**, dedicated to the public domain by Ryan Wolfslayer (see [LICENSE](LICENSE)).

You are free to copy, modify, distribute and use these translations for any purpose without attribution or permission — as a text, as data, or as the starting point for your own translation or edition. Attribution to *Bibliothecarius Modernus* is appreciated, not required.

Note: some older YouTube descriptions and the Zenodo records deposited in 2025 state CC BY 4.0; they are not edited retroactively. The CC0 dedication of the same content is the operative statement for reuse.

## Manuscript transcriptions (future)

Where a neglected work survives only in manuscript, or no usable printed text exists, the library will transcribe it from digitised images held by libraries and museums. Such a transcription arrives here as `Latin/*.txt` with a `Latin/transcription_provenance.json` beside it (schema `bibliothecarius.transcription_provenance/1`) recording: creator (Bibliothecarius Modernus), date, the holding institution, shelfmark and folio range, the source-image or IIIF URL and the images' rights statement, the transcription method and model, the normalization policy, the review status, known uncertainties, and a version. The transcription is **CC0 1.0** like every other Bibliothecarius contribution, versioned, and accompanied by its provenance and review information so that credit and blame for this specific digital text are explicit. The manuscript images themselves are not part of the corpus and are never represented as CC0: they remain under the terms of the institution that holds them, which is credited first and fully wherever an image is reproduced.

## How the corpus is produced

Editions are produced by the library's pipeline: source extraction with boundaries read by the curator, AI-assisted translation in short source-anchored segments, deterministic coverage checks, cross-family review, recorded corrections, narration, subtitles and video, then publication to this repository, the website, YouTube and Archive.org, with the catalog record written last. The method, standards and decision record are described on the [About page](https://bibliothecarius-modernus.github.io/about/) and in the project white paper (DOI [10.5281/zenodo.18002473](https://doi.org/10.5281/zenodo.18002473), December 2025; CC BY 4.0).

## The library elsewhere

- Website (reading room: parallel text, introduction, bibliography, Resource Info, search in Latin and English): https://bibliothecarius-modernus.github.io
- YouTube (archival video editions — the Latin on screen, the English read aloud): https://www.youtube.com/@BibliothecariusModernus
- Internet Archive (audio editions and edition data): https://archive.org/details/@ryan_wolfslayer
- Machine-readable catalog: https://bibliothecarius-modernus.github.io/api/catalog.json — documentation https://bibliothecarius-modernus.github.io/api/README.md
- White paper (2025): https://doi.org/10.5281/zenodo.18002473

## Contributing

Corrections, references to existing scholarly translations or editions, and requests for works are welcome: open an issue or a pull request, or write to bibliothecarius.modernus@gmail.com. Translations are not hand-edited in place; a correction is recorded with its Latin basis and applied by the pipeline so that the edition's provenance stays complete.
