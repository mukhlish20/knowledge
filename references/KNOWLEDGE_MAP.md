# Knowledge Map

This document defines the bundled reference layout for the **Komikus** children's-comic skill.

## Package Layout

The skill package keeps `SKILL.md` at the package root and stores reference material in sibling directories:

```
SKILL.md
hadith/
quran/
tafsir/
references/
```

Paths below are therefore **package-relative**. Do not prepend `knowledge/`.

## Qur'an

- `quran/quran-uthmani.txt` — primary Arabic Qur'an text.
- `quran/id.indonesian.txt` — Indonesian translation.
- `quran/quran-data.xml` — structural Qur'an metadata.

## Tafsir

- `tafsir/id.jalalayn.txt` — Tafsir Jalalayn. Treat tafsir as explanation/context, never as Qur'an text or a literal translation.

## Hadith

The bundled hadith collections are consolidated into one JSON file per collection:

- `hadith/riyadhus_shalihin.json` — Riyadhus Shalihin.
- `hadith/al_adab_al_mufrad.json` — Al-Adab Al-Mufrad.
- `hadith/bulugh_al_maram.json` — Bulugh al-Maram.

Use the structured metadata and Arabic/source text contained in these files when permitted for redistribution.

For distributable packages, include only hadith material whose redistribution rights are explicitly verified. Third-party English translations sourced from Sunnah.com are not assumed to be redistributable merely because structured dataset metadata is CC0.

## Retrieval Rules

1. Prefer exact bundled source text for religious quotations.
2. Use metadata for identification, navigation, collection, and reference numbers.
3. Never reconstruct Qur'an or hadith quotations from model memory when the exact bundled text is available.
4. Never present an AI paraphrase as an exact quotation.
5. Keep Qur'an text, translation, tafsir, hadith text, narrator information, grading, and commentary conceptually distinct.
6. If exact verification is unavailable, do not invent or guess a quotation or reference number.
