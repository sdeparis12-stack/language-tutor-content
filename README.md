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

## Lesson 1AD.1 — Dar: present and past

Follows 1AC.1's six-stage, 44-step structure with doy / damos and di / dimos.
Practice covers giving answers, tips, gifts, and explanations, alongside the
common expressions dar un paseo (take a walk) and dar las gracias (say thank you).
The supported gift sentence introduces le with an explicit recipient, mi hermana.

The progression is 6 Spanish Easy introductions, 6 English Medium attempts with
only the dar form hidden, 8 short English Hard switches, 12 present/past
English Hard switches, 6 Spanish Easy mixed sentences, and 6 English Hard mixed
recall attempts: 32 phrase-bank entries and 44 attempts, including 26 Hard.
New content vocabulary appears in supported Spanish before recall.

Each sentence has one canonical answer and one primary dar target. Ir, tener,
hacer, estar, decir, and poder return as context in the final section. Other
verbs are not separate primary targets; the app still expects every word of the
canonical sentence under its existing word-coverage grading.

The lesson follows 1AC.1 under Verb Practice. Catalog revision 13 adds it without
changing earlier packs or versions. Validation covers the app's parser, grader,
masks, runner, and catalog checks, including 44 canonical answers and 132
wrong-form checks. Wrong-form substitutions match whole words so di does not
alter dije. Live speech recognition remains a device-level check.

## Lesson 1AE.1 — Ver: present and past

Follows 1AD.1's six-stage, 44-step structure with veo / vemos and vi / vimos.
Practice covers movies, museum exhibitions, family, friends, trip photographs,
and phone messages. Seeing a specific person uses the personal a, introduced
in supported phrases before recall. Ver una película is translated naturally
as "watch a movie." Each prompt has one canonical Spanish answer.

The progression is 6 Spanish Easy introductions, 6 English Medium attempts with
only the ver form hidden, 8 short English Hard switches, 12 present/past
English Hard switches, 6 Spanish Easy mixed sentences, and 6 English Hard mixed
recall attempts: 32 phrase-bank entries and 44 attempts, including 26 Hard.
New content vocabulary appears in supported Spanish before recall.

Each sentence has one primary ver target. Ir, tener, hacer, estar, dar, and poder
return as context in the final section. Other verbs are not separate primary
targets; the app still expects every word of the canonical sentence under its
existing word-coverage grading.

The lesson follows 1AD.1 under Verb Practice. Catalog revision 16 adds it while
preserving all 14 previous lesson entries, including Visiting Friends version 2.
Validation covers the app's parser, grader, masks, runner, and catalog checks,
including 44 canonical answers and 132 whole-word wrong-form checks. Live speech
recognition remains a device-level check.

## Lesson 1AF.1 — Decir: present and past

Follows the established six-stage, 44-step structure with digo / decimos and
dije / dijimos: 12 Spanish Easy, 6 English Medium, and 26 English Hard attempts.
Decir previously appeared as context; this is its first dedicated Drill pack.
Practice includes telling the truth, saying names and addresses, brief remarks,
saying nothing, and communicating a meeting time.

The six longer sentences deliberately vary their structure: a why-question, a
negative with a reason, a time phrase before reported speech, a contrast with
pero, a message report, and an embedded where-clause. They revisit poder, ver,
ir, dar, traer, and poner in a different order. New words and structures first
appear in Spanish Easy. Final Hard recall uses the fixed mixed order p30, p27,
p32, p28, p31, p29 rather than replaying the exposure order. Each sentence still
has one canonical answer and one primary decir target.

Authoring preference for subsequent lessons: vary the longer sentence openings,
clause structures, situations, maintenance verbs, and yo/nosotros order. Avoid
repeatedly using "Tuvimos tiempo," "Pudimos salir," or "Estuvimos" as a template.
Use deliberate variety with supported exposure; keep published sequence order
stable for resume and progress. This is authored variety, not runtime shuffling.

Catalog revision 17 appends the lesson after 1AE.1 in Verb Practice and preserves
all 15 prior lesson entries, including Visiting Friends version 2. Validation
covers 44 canonical answers, 132 wrong-form checks, masks, full completion, and
next-lesson navigation. Live speech recognition remains a device-level check.

## Lessons 1AG.1–1AK.1 — Five-verb practice batch

| Lesson | Focus | Present: yo / nosotros | Preterite: yo / nosotros |
| --- | --- | --- | --- |
| 1AG.1 | Querer | quiero / queremos | quise / quisimos |
| 1AH.1 | Saber | sé / sabemos | supe / supimos |
| 1AI.1 | Hablar | hablo / hablamos | hablé / hablamos |
| 1AJ.1 | Salir | salgo / salimos | salí / salimos |
| 1AK.1 | Llegar | llego / llegamos | llegué / llegamos |

Querer and salir refresh the learner's earlier Voice Mode practice. Each pack
keeps the six-stage structure: 12 Spanish Easy, 6 English Medium, and 26 English
Hard attempts. The batch supplies 220 attempts, including 130 Hard attempts.
Each sentence has one canonical answer and one primary target; other verbs
provide context, while the app still expects the whole canonical sentence.

Saber contrasts knowing now with finding out in the past: sé / sabemos versus
supe / supimos. Querer practices bounded past wants, with no quise / no quisimos
translated as refusal in the selected examples. These are contextual meanings,
not universal word-for-word substitution rules.

Hablamos, salimos, and llegamos share their present and preterite surface forms.
Time cues distinguish the intended readings, and target metadata keeps their
person and tense separate. A shared surface form is never listed as its own
competing answer. Background imperfect forms había and hacía in the supported noise and weather
sentences are context, not new primary targets.

The longer sections vary questions, reasons, contrasts, time clauses, reported
information, destinations, and everyday situations. New vocabulary appears with
Spanish support before English recall. Each final Hard section uses a distinct,
fixed mixed order so practice is less predictable while resume stays stable.

Catalog revision 18 appends all five after 1AF.1 in Verb Practice, preserving all
16 existing lesson entries, versions, and files, including Visiting Friends v2.
Validation covers 220 canonical answers, 528 wrong-form substitutions, masks,
target tense and person, full completion, and navigation between lessons. These
checks do not simulate live speech recognition.

Suggested follow-up: two unit reviews, one mixing irregular verbs and another
combining verbs in everyday situations. Those reviews are not part of this batch.

## Unit Review 1 — Mixed Verbs: Present & Past

The first cumulative review is listed directly after 1AK.1 under Verb Practice.
Its title starts with **Unit Review 1** so it is distinct from individual verb
lessons. The subtitle is **Easy → Medium → Hard · 48 exercises**. Future reviews
should use the same `Unit Review N —` prefix and stable `unit_review_NN_...` ID.

Version 2 gives the review a gentler progression: 16 selected phrases, each
practiced in Easy, Medium, and Hard. Two rounds keep the supported practice close
to recall. Each round mixes verbs, and each support level uses a different fixed
order so the next answer cannot be inferred from the preceding sequence.

| Round | Spanish Easy | English Medium | English Hard |
| --- | ---: | ---: | ---: |
| Short mixed foundations | 8 | 8 | 8 |
| Contrasts and connections | 8 | 8 | 8 |

Easy shows the complete Spanish sentence. Medium hides only the primary verb
form while leaving the rest of the sentence visible. Hard hides the full Spanish
sentence. Every Hard sentence in this revision has already appeared in both
Easy and Medium within the same round. There are 48 attempts, including only
16 Hard attempts, rather than the original jump from 6 Easy to 26 Hard.

The main focus remains querer, saber, hablar, salir, and llegar, with dar, ver,
and decir as reinforcement. Knowing versus finding out, wanting versus refusing,
and present/past nosotros forms return in separate rounds. Each sentence has one
canonical answer and one primary tracked target. Other verbs provide context;
the app still checks full-sentence word coverage. Shared present/past surface
forms use time cues and distinct target metadata and never compete with themselves.

Authoring preference for future lessons and reviews: preview the focus forms and
key learning vocabulary in Easy or Medium before Hard. Exact sentence previews
are useful but not mandatory everywhere. Familiar vocabulary substitutions and
occasional new material are welcome as stretch goals. Keep the overall progression
supportive; do not treat this preference as an absolute ban on novelty in Hard.
This revision deliberately previews every complete sentence to ease back into recall.

Catalog revision 20 updates this existing review to lessonVersion 2, retaining its
canonical ID, title, directory entry, and all other lesson files and versions.
The app retains history under the same lesson ID. A saved run from version 1 cannot
resume against the new sequence; the app asks for a restart and keeps earlier results.

Validation covers 48 canonical answers, 123 wrong-form substitutions, Medium masks,
prior Easy/Medium exposure for every Hard phrase, target metadata, two resume cases,
full completion, and navigation after 1AK.1. Download and offline loading use the
production content path. Live speech recognition remains a device-level check.
Dynamic retries and Unit Review 2 are future work.
