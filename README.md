# Language Tutor Lesson Content

Public lesson files for the Language Tutor app. This repository contains lesson
Markdown, the versioned manifest, and the authored navigation directory.

The app retrieves `lesson_manifest.json` over ordinary HTTPS. Lesson paths and
`directoryFile` are relative to that manifest. Navigation comes from the authored
directory, not physical folders.

## Publishing changes

1. Author and validate the Markdown pack with the app’s existing lesson validator.
2. Keep the canonical lesson ID when editing an existing lesson. Increment its
   `lessonVersion` in the pack and manifest when its content changes.
3. Calculate the SHA-256 of the exact Markdown bytes (for example,
   `shasum -a 256 Lessons/venir-01.md`) and update its manifest entry.
4. Add or update directory references. Cross-listed entries share a canonical
   lesson ID and use distinct entry IDs.
5. Increment `catalogRevision` in both JSON files to the same higher number.
6. Commit and push the complete content set, then use Refresh Lessons in the app.

The app activates only a fully validated catalog and retains its prior local copy
when a download or validation fails. Learner progress stays local to the app.
To roll back content, publish the restored content with a new higher catalog
revision and correct hashes rather than lowering the revision.

## Bootstrap URL

https://raw.githubusercontent.com/sdeparis12-stack/language-tutor-content/main/lesson_manifest.json

## Lesson 1W series

All three lessons appear together under **Verb Practice**. Each item has one
canonical Spanish answer; repeat that answer exactly. Traer is the primary focus.
Venir, decir, object pronouns, and embedded imperfect forms are context rather
than separately tracked targets; the app still checks the complete sentence.

- **1W.1 — Traer: present and past**: original items 1–30, plus the supported coat
  vocabulary repair (31 steps). This existing lesson is unchanged.
- **1W.2 — Traer: vocabulary and connections**: original items 31–58 (28 steps).
  Spanish Easy introduces each group; English Medium hides the traer form only.
  Covers dessert, luggage, photographs, and combinations with venir and decir.
- **1W.3 — Traer: stories and tense switching**: original items 59–76, with six
  Spanish Easy exposures before the 18 English Hard recall items (24 steps).
  The support covers phone/only, later, “todo lo que necesitábamos,” “quería tomar
  fotos,” and “esta vez.” The full original answers for items 66 and 67 are the
  canonical answers; shorter alternatives and Voice Mode directions are omitted.

When a sentence contains both present and past traer forms, its past form is the
single tracked primary target. Other correctly expected traer forms are excluded
from competing-form metadata. The final mixed challenge retains its original
sentence order, wording, and full-sentence recall requirement.

Catalog revision 5 adds 1W.2 and 1W.3 without changing earlier lesson IDs, versions,
content, or progress. Publication was checked with the app's production parser,
validator, grader, runner, cache, and content-sync path. All 52 new steps were
checked for exact source wording, masks, canonical-answer success, and rejection
of a wrong primary traer form. These checks do not simulate live speech recognition.
