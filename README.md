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

## Lesson 1Y.1 — Tener: present and past

Follows 1X.1's six-stage, 44-step structure exactly, using tengo / tenemos and
tuve / tuvimos as the four primary forms. Practice includes meetings, appointments,
time, car problems, luck, and doubts. New content vocabulary first appears in
supported Spanish; familiar present forms and time markers are used for switching.

| Stage | Prompt and support | Steps |
| --- | --- | ---: |
| Supported past introduction | Spanish Easy | 6 |
| Simple past recall | English Medium; only the tener form hidden | 6 |
| Short past switching | English Hard | 8 |
| Present/past switching | English Hard | 12 |
| Supported cumulative mix | Spanish Easy | 6 |
| Cumulative past recall | English Hard | 6 |

Each sentence has one canonical answer and one primary tener target. Venir, decir,
traer, and poner reappear as context in the final mixed section; they do not gain
separate target tracking. The whole sentence still needs to match the displayed
canonical answer. There are 32 phrase-bank entries and 44 total attempts, including
26 Hard attempts. The lesson appears directly after 1X.1 under Verb Practice.

Catalog revision 8 adds this lesson without changing existing packs or their
versions. Validation uses the app's production parser, grader, masks, runner, and
catalog checks, including 44 canonical answers and 132 wrong-form checks. Live
speech recognition remains a device-level check.

## Lesson 1Z.1 — Estar: present and past

Follows 1Y.1's six-stage, 44-step structure with estoy / estamos and
estuve / estuvimos. Practice focuses on where you are today and where you were
during a completed past visit. Locations include the office, museum, pharmacy,
station, home, and park. New content vocabulary appears in supported Spanish
before recall; familiar present forms and time markers support tense switching.

The progression is 6 Spanish Easy introductions, 6 English Medium attempts with
only the estar form hidden, 8 short English Hard switches, 12 present/past
English Hard switches, 6 Spanish Easy mixed sentences, and 6 English Hard mixed
recall attempts: 32 phrase-bank entries and 44 attempts, including 26 Hard.

Each sentence has one canonical answer and one primary estar target. Venir,
traer, decir, and tener return as context in the mixed section; the app still
checks the whole canonical sentence. The lesson follows 1Y.1 under Verb Practice.

Catalog revision 9 adds this lesson without changing earlier packs or versions.
Validation uses the app's production parser, grader, masks, runner, and catalog
checks, including all 44 canonical answers and 132 wrong-form checks. Live speech
recognition remains a device-level check.

## Lesson 1AA.1 — Hacer: present and past

Follows 1Z.1's six-stage, 44-step structure with hago / hacemos and hice / hicimos.
Practice covers making meals, making plans and reservations, asking questions,
and exercising. New content vocabulary appears in supported Spanish before
recall; present forms and familiar time markers support tense switching.

The progression is 6 Spanish Easy introductions, 6 English Medium attempts with
only the hacer form hidden, 8 short English Hard switches, 12 present/past
English Hard switches, 6 Spanish Easy mixed sentences, and 6 English Hard mixed
recall attempts: 32 phrase-bank entries and 44 attempts, including 26 Hard.

Each sentence has one canonical answer and one primary hacer target. The final
section revisits venir, traer, decir, poner, tener, and estar as context, while
the app still checks the whole canonical sentence. In combinations such as
"vine temprano e hice la cena," e means "and": y becomes e before the initial
/i/ sound in hice and hicimos. These combinations appear with Spanish support
before recall. English translations use natural phrasing, so hacer una pregunta
is "ask a question" and hacer ejercicio is "exercise."

The lesson follows 1Z.1 under Verb Practice. Catalog revision 10 adds this lesson
without changing earlier packs or versions. Validation uses the app's production
parser, grader, masks, runner, and catalog checks, including all 44 canonical
answers and 132 wrong-form checks. Live speech recognition remains a device-level
check.

## Lesson 1AB.1 — Poder: present and past

Follows 1AA.1's six-stage, 44-step structure with puedo / podemos and pude /
pudimos. Practice covers finishing work, reservations, getting to meetings,
buying tickets, opening a door, and finding keys. Positive past examples use
"was/were able to" for achieved actions; negative examples practice no pude /
no pudimos. The infinitive after poder stays unchanged.

The progression is 6 Spanish Easy introductions, 6 English Medium attempts with
only the poder form hidden, 8 short English Hard switches, 12 present/past
English Hard switches, 6 Spanish Easy mixed sentences, and 6 English Hard mixed
recall attempts: 32 phrase-bank entries and 44 attempts, including 26 Hard.
New content vocabulary appears in supported Spanish before recall.

Each sentence has one canonical answer and one primary poder target. Familiar
venir, tener, traer, estar, hacer, and decir forms return in the mixed section
as context; the app still checks the complete canonical sentence.

The lesson follows 1AA.1 under Verb Practice. Catalog revision 11 adds it without
changing earlier packs or versions. Validation covers the app's parser, grader,
masks, runner, and catalog checks, including 44 canonical answers and 132
wrong-form checks. Live speech recognition remains a device-level check.

## Lesson 1AC.1 — Ir: present and past

Follows 1AB.1's six-stage, 44-step structure with voy / vamos and fui / fuimos.
The focus is going to places: the supermarket, station, pharmacy, museum, office,
and park. Destination phrases reinforce a la and al. All uses of fui / fuimos
in this pack mean "went"; the shared ser forms are not introduced here.

The progression is 6 Spanish Easy introductions, 6 English Medium attempts with
only the ir form hidden, 8 short English Hard switches, 12 present/past
English Hard switches, 6 Spanish Easy mixed sentences, and 6 English Hard mixed
recall attempts: 32 phrase-bank entries and 44 attempts, including 26 Hard.
New content vocabulary appears in supported Spanish before recall.

Each sentence has one canonical answer and one primary ir target. Hacer, tener,
poder, traer, decir, and estar return as context in the final section. Other
verbs are not separate primary targets; the app still expects every word of the
canonical sentence under its existing word-coverage grading.

The lesson follows 1AB.1 under Verb Practice. Catalog revision 12 adds it without
changing earlier packs or versions. Validation covers the app's parser, grader,
masks, runner, and catalog checks, including 44 canonical answers and 132
wrong-form checks. Live speech recognition remains a device-level check.
