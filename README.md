# Latin Patristic Texts

Welcome to the Latin Patristic Texts repository! This repository houses plain text files of Latin Patristic works that have been translated using modern AI technology. These texts are part of a personal project to make classical Church history more accessible.

## Repository Structure

```
Patrologia_Latina/
├── README.md                             # Works catalog
└── vol_XXX/                              # Volume number from Migne's Patrologia Latina
    └── Author Name - Work Title/
        ├── Latin/
        │   └── *.txt                     # Original Latin text (public domain)
        ├── Author-Name-Work-Title-Full-Text-Edition.txt
        │                                 # Combined English translation
        └── translation.json              # Structured metadata (newer works only)
```

Production artifacts for YouTube video generation (`SSML/`, `Subtitles/`) may also be present in work directories.

## About the Translations

Translations were generated using AI (Claude, GPT-4) and should be treated as introductory guides rather than scholarly editions. Audio versions were produced using OpenAI TTS and Amazon Polly.

## License

Owner decision (Bibliothecarius Modernus v2, 2026-09-13), stated the same way on the website, Archive.org and in every new `translation.json`:

- **Latin texts** (`Latin/*.txt`, `source.txt`, the `latin` field of `translation.json` chunks): **public-domain source material** — J.-P. Migne, *Patrologia Latina* (1844–65), reproduced as extracted for the parallel translation. No rights are claimed over the Latin; where this project contributed transcription or markup, those contributions are dedicated CC0 as below. The underlying digitised database is not redistributed here.
- **Everything Bibliothecarius Modernus created** — the English translations, full-text editions, `translation.json` metadata and notes, subtitles, SSML and any other scholarly contribution in this repository: **[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)**, dedicated to the public domain by Ryan Wolfslayer (see [LICENSE](LICENSE)).

You are free to copy, modify, distribute and use these translations for any purpose without attribution or permission. Attribution to *Bibliothecarius Modernus* is appreciated, not required.

Note: some older YouTube descriptions and the Zenodo records deposited in 2025 state CC BY 4.0; they are not edited retroactively. The CC0 dedication of the same content is the operative statement for reuse.

## Contributing

Contributions are welcome! If you have texts to add or improvements to suggest, please open an issue or submit a pull request.

## About

This repository is part of the Bibliothecarius Modernus - The Modern Librarian project, dedicated to making ancient texts accessible through modern technology. For more information, visit our [YouTube channel](https://www.youtube.com/channel/UC5hvJMbDPhlh2ldZPe_CgOg).
