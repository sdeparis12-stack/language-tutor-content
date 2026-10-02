---
schemaVersion: 1
lessonId: lesson_1w_2_traer_connections
lessonVersion: 1
mode: drill
title: "1W.2 — Traer: vocabulary and connections"
primaryTargets:
  - id: traer-yo-preterite
    form: traje
    lemma: traer
    person: yo
    tense: preterite
  - id: traer-nosotros-preterite
    form: trajimos
    lemma: traer
    person: nosotros
    tense: preterite
  - id: traer-yo-present
    form: traigo
    lemma: traer
    person: yo
    tense: present
  - id: traer-nosotros-present
    form: traemos
    lemma: traer
    person: nosotros
    tense: present
---

# Phrase Bank

## phrase: p31
Spanish: "Ayer traje un postre para todos."
English: "Yesterday I brought a dessert for everyone."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p32
Spanish: "Trajimos nuestro equipaje en el coche."
English: "We brought our luggage in the car."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p33
Spanish: "Traje una foto para enseñársela a mi amigo."
English: "I brought a photograph to show my friend."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p34
Spanish: "Trajimos una linterna porque estaba oscuro."
English: "We brought a flashlight because it was dark."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p35
Spanish: "Hoy traigo mi cámara otra vez."
English: "Today I’m bringing my camera again."
Targets:
  - traer-yo-present
CompetingTargetForms:
  - traje
  - trajimos
  - traemos

## phrase: p36
Spanish: "Hoy traemos las herramientas porque podemos ayudar."
English: "Today we’re bringing the tools because we can help."
Targets:
  - traer-nosotros-present
CompetingTargetForms:
  - traje
  - trajimos
  - traigo

## phrase: p37
Spanish: "Ayer traje un postre para todos."
English: "Yesterday I brought dessert for everyone."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p40
Spanish: "Ayer trajimos una linterna."
English: "Yesterday we brought a flashlight."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p41
Spanish: "Hoy traemos las herramientas."
English: "Today we’re bringing the tools."
Targets:
  - traer-nosotros-present
CompetingTargetForms:
  - traje
  - trajimos
  - traigo

## phrase: p42
Spanish: "Traje una foto ayer."
English: "I brought a photograph yesterday."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p43
Spanish: "Ayer vine en coche y traje mi cámara."
English: "Yesterday I came by car and brought my camera."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p44
Spanish: "Vinimos temprano y trajimos todo."
English: "We came early and brought everything."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p45
Spanish: "Hoy vengo en tren y traigo mi libreta."
English: "Today I’m coming by train and bringing my notebook."
Targets:
  - traer-yo-present
CompetingTargetForms:
  - traje
  - trajimos
  - traemos

## phrase: p46
Spanish: "Hoy venimos temprano y traemos las herramientas."
English: "Today we’re coming early and bringing the tools."
Targets:
  - traer-nosotros-present
CompetingTargetForms:
  - traje
  - trajimos
  - traigo

## phrase: p51
Spanish: "Ayer dije que traje todo."
English: "Yesterday I said that I brought everything."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p52
Spanish: "Dijimos que trajimos nuestra cámara."
English: "We said that we brought our camera."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p53
Spanish: "Hoy digo que traigo mi cargador."
English: "Today I say that I’m bringing my charger."
Targets:
  - traer-yo-present
CompetingTargetForms:
  - traje
  - trajimos
  - traemos

## phrase: p54
Spanish: "Decimos que traemos el postre."
English: "We say that we’re bringing dessert."
Targets:
  - traer-nosotros-present
CompetingTargetForms:
  - traje
  - trajimos
  - traigo

# Stages

## stage: supported-vocabulary
PromptLanguage: spanish
Difficulty: easy
Phrases:
  - p31
  - p32
  - p33
  - p34
  - p35
  - p36

## stage: vocabulary-recall
PromptLanguage: english
Difficulty: medium
Phrases:
  - p37
  - p32
  - p35
  - p40
  - p41
  - p42
Masks:
  p37:
    - traje
  p32:
    - trajimos
  p35:
    - traigo
  p40:
    - trajimos
  p41:
    - traemos
  p42:
    - traje

## stage: supported-venir-combinations
PromptLanguage: spanish
Difficulty: easy
Phrases:
  - p43
  - p44
  - p45
  - p46

## stage: venir-combination-recall
PromptLanguage: english
Difficulty: medium
Phrases:
  - p43
  - p44
  - p45
  - p46
Masks:
  p43:
    - traje
  p44:
    - trajimos
  p45:
    - traigo
  p46:
    - traemos

## stage: supported-decir-combinations
PromptLanguage: spanish
Difficulty: easy
Phrases:
  - p51
  - p52
  - p53
  - p54

## stage: decir-combination-recall
PromptLanguage: english
Difficulty: medium
Phrases:
  - p51
  - p52
  - p53
  - p54
Masks:
  p51:
    - traje
  p52:
    - trajimos
  p53:
    - traigo
  p54:
    - traemos

