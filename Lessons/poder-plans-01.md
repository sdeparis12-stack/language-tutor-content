---
schemaVersion: 1
lessonId: lesson_poder_plans_01
lessonVersion: 1
mode: drill
title: "Poder — Making plans"
primaryTargets:
  - id: poder-plans-yo-present
    form: puedo
    lemma: poder
    person: yo
    tense: present
  - id: poder-plans-nosotros-present
    form: podemos
    lemma: poder
    person: nosotros
    tense: present
---

# Phrase Bank

## phrase: poder-plans-01
Spanish: Puedo estudiar esta tarde.
English: I can study this afternoon.
Targets:
  - poder-plans-yo-present
CompetingTargetForms:
  - podemos

## phrase: poder-plans-02
Spanish: Podemos hablar mañana.
English: We can talk tomorrow.
Targets:
  - poder-plans-nosotros-present
CompetingTargetForms:
  - puedo

# Stages

## stage: exposure
PromptLanguage: spanish
Difficulty: easy
Phrases: all

## stage: supported-recall
PromptLanguage: english
Difficulty: medium
Phrases:
  - poder-plans-02
  - poder-plans-01
Masks:
  poder-plans-01:
    - puedo
    - tarde
  poder-plans-02:
    - podemos
    - mañana

## stage: independent-recall
PromptLanguage: english
Difficulty: hard
Phrases: all
