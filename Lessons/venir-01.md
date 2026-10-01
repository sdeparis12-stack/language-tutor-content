---
schemaVersion: 1
lessonId: lesson_venir_01
lessonVersion: 1
mode: drill
title: "Venir — Talking about yesterday"
primaryTargets:
  - id: venir-yo-past
    form: vine
    lemma: venir
    person: yo
    tense: preterite
  - id: venir-nosotros-past
    form: vinimos
    lemma: venir
    person: nosotros
    tense: preterite
---

# Phrase Bank

## phrase: venir-01
Spanish: Vine a casa ayer.
English: I came home yesterday.
Targets:
  - venir-yo-past
CompetingTargetForms:
  - vinimos

## phrase: venir-02
Spanish: Vinimos juntos el lunes.
English: We came together on Monday.
Targets:
  - venir-nosotros-past
CompetingTargetForms:
  - vine

# Stages

## stage: exposure
PromptLanguage: spanish
Difficulty: easy
Phrases: all

## stage: supported-recall
PromptLanguage: english
Difficulty: medium
Phrases:
  - venir-02
  - venir-01
Masks:
  venir-01:
    - vine
    - ayer
  venir-02:
    - vinimos
    - juntos

## stage: independent-recall
PromptLanguage: english
Difficulty: hard
Phrases: all
