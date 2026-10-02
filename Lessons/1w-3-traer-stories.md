---
schemaVersion: 1
lessonId: lesson_1w_3_traer_stories
lessonVersion: 1
mode: drill
title: "1W.3 — Traer: stories and tense switching"
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

## phrase: p59
Spanish: "Ayer traje la cámara, pero hoy traigo mi teléfono."
English: "I brought the camera yesterday, but today I’m bringing my phone."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traemos

## phrase: p60
Spanish: "Ayer trajimos todo, pero hoy traemos solamente las herramientas."
English: "We brought everything yesterday, but today we’re bringing only the tools."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo

## phrase: p62
Spanish: "Hoy vengo más tarde y traigo mi cámara."
English: "Today I’m coming later and bringing my camera."
Targets:
  - traer-yo-present
CompetingTargetForms:
  - traje
  - trajimos
  - traemos

## phrase: p66
Spanish: "Vinimos en coche y trajimos todo lo que necesitábamos."
English: "We came by car and brought everything we needed."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p67
Spanish: "Dije que traje mi cámara porque quería tomar fotos."
English: "I said that I brought my camera because I wanted to take photos."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p69
Spanish: "Hoy vengo otra vez, pero esta vez traigo mi abrigo."
English: "Today I’m coming again, but this time I’m bringing my coat."
Targets:
  - traer-yo-present
CompetingTargetForms:
  - traje
  - trajimos
  - traemos

## phrase: p61
Spanish: "Ayer vine temprano y traje mi libreta."
English: "Yesterday I came early and brought my notebook."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p63
Spanish: "Dijimos que vinimos en coche y trajimos todo."
English: "We said that we came by car and brought everything."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p64
Spanish: "Hoy decimos que venimos en tren y traemos nuestro equipaje."
English: "Today we say that we’re coming by train and bringing our luggage."
Targets:
  - traer-nosotros-present
CompetingTargetForms:
  - traje
  - trajimos
  - traigo

## phrase: p65
Spanish: "Ayer vine a las seis y traje un postre."
English: "Yesterday I came at six and brought dessert."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p68
Spanish: "Dijimos que trajimos una linterna porque estaba oscuro."
English: "We said that we brought a flashlight because it was dark."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo
  - traemos

## phrase: p70
Spanish: "Venimos otra vez mañana y traemos el postre."
English: "We’re coming again tomorrow and bringing dessert."
Targets:
  - traer-nosotros-present
CompetingTargetForms:
  - traje
  - trajimos
  - traigo

## phrase: p71
Spanish: "Lo traigo hoy; lo traje ayer."
English: "I bring it today; I brought it yesterday."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traemos

## phrase: p72
Spanish: "Lo traemos hoy; lo trajimos ayer."
English: "We bring it today; we brought it yesterday."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo

## phrase: p73
Spanish: "Ayer vine y traje todo; hoy vengo otra vez y traigo solamente mi cámara."
English: "I came yesterday and brought everything; today I’m coming again and bringing only my camera."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traemos

## phrase: p74
Spanish: "Ayer dijimos que trajimos todo, pero hoy decimos que traemos más."
English: "We said yesterday that we brought everything, but today we say that we’re bringing more."
Targets:
  - traer-nosotros-preterite
CompetingTargetForms:
  - traje
  - traigo

## phrase: p75
Spanish: "Ayer dije que vine en tren y traje mi libreta."
English: "Yesterday I said I came by train and brought my notebook."
Targets:
  - traer-yo-preterite
CompetingTargetForms:
  - trajimos
  - traigo
  - traemos

## phrase: p76
Spanish: "Hoy digo que vengo en coche y traigo las herramientas."
English: "Today I say that I’m coming by car and bringing the tools."
Targets:
  - traer-yo-present
CompetingTargetForms:
  - traje
  - trajimos
  - traemos

# Stages

## stage: supported-story-wording
PromptLanguage: spanish
Difficulty: easy
Phrases:
  - p59
  - p60
  - p62
  - p66
  - p67
  - p69

## stage: mixed-present-past-recall
PromptLanguage: english
Difficulty: hard
Phrases:
  - p59
  - p60
  - p61
  - p62
  - p63
  - p64

## stage: visiting-friends-story
PromptLanguage: english
Difficulty: hard
Phrases:
  - p65
  - p66
  - p67
  - p68
  - p69
  - p70

## stage: final-switching-challenge
PromptLanguage: english
Difficulty: hard
Phrases:
  - p71
  - p72
  - p73
  - p74
  - p75
  - p76

