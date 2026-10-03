# Knowledge Map

This document defines the **lightweight reference/index layer** for the Komikus children's-comic Skill.

## Package Layout

The distributable Skill package intentionally contains only:

```
SKILL.md
references/
└── KNOWLEDGE_MAP.md
```

Large raw Qur'an, tafsir, and hadith datasets are **not bundled** in the Skill ZIP. They can make the package unnecessarily large and are not required for the Skill's core comic-generation workflow.

## Religious Knowledge Sources

The Skill may use religious sources that are explicitly provided or connected by the user/runtime.

Recommended source roles:

- Qur'an: verified Qur'an text plus a clearly identified Indonesian translation when needed.
- Tafsir: use only as explanation/context; never present tafsir as Qur'an text or a literal translation.
- Hadith: identify the collection, reference/number, narrator, grading, and commentary separately when those details are verified.

The following collections are useful conceptual source categories when available:

- Riyadhus Shalihin — moral and spiritual themes.
- Al-Adab Al-Mufrad — manners, parents, children, neighbours, compassion, and social behavior.
- Bulugh al-Maram — worship and ahkam-oriented subjects.

These names are **source guidance, not bundled files**.

## Retrieval and Integrity Rules

1. Prefer an explicitly provided or connected verified source for exact religious quotations.
2. Never reconstruct Qur'an or hadith quotations from model memory and label them as exact.
3. Never present an AI paraphrase as an exact quotation.
4. Keep Qur'an text, translation, tafsir, hadith text, narrator information, grading, and commentary conceptually distinct.
5. If exact verification is unavailable, do not invent or guess a quotation, citation, or reference number.
6. If the user needs an exact quotation, explain the verification limitation and use a verifiable source when one is available.

## Package Design Principle

The Skill package should remain small and focused on **behavior, workflow, continuity, story design, and source-integrity rules**. Large reference corpora belong outside the distributable Skill package unless the target platform explicitly supports and requires them.
