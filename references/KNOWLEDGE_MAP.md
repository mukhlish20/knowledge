# Knowledge Map

This document explains the bundled reference layout for the children's-comic-generator skill.

## Quran
- `knowledge/quran/quran-uthmani.txt` — primary Arabic Quran text.
- `knowledge/quran/id.indonesian.txt` — Indonesian translation.
- `knowledge/quran/quran-data.xml` — structural Quran metadata.

## Tafsir
- `knowledge/tafsir/id.jalalayn.txt` — Tafsir Jalalayn. Treat tafsir as explanation/context, never as Quran text or literal translation.

## Hadith
- `knowledge/hadith/riyadhus_shalihin/` — Riyadhus Shalihin.
- `knowledge/hadith/al_adab_al_mufrad/` — Al-Adab Al-Mufrad.
- `knowledge/hadith/bulugh_al_maram/` — Bulugh al-Maram.

For distributable packages, include only hadith material whose redistribution rights are explicitly verified. Third-party English translations sourced from Sunnah.com are not assumed to be redistributable merely because structured dataset metadata is CC0.

## Retrieval rule
Prefer exact bundled source text for religious quotations. Use metadata for identification and navigation. Never reconstruct Quran or hadith quotations from model memory when the exact bundled text is available.
