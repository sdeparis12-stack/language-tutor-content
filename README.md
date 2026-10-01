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
