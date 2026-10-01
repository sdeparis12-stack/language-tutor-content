---
schemaVersion: 1
lessonId: "prototype-2f-poder-present"
lessonVersion: 2
mode: drill
title: "Poder: supported exposure to English recall"
language:
  learning: es-MX
  interface: en-US
primaryTargets:
  - id: puedo
    form: puedo
    lemma: poder
    person: yo
    tense: present
  - id: podemos
    form: podemos
    lemma: poder
    person: nosotros
    tense: present
---

# Phrase Bank

## phrase: poder-01

Spanish: Puedo ir al restaurante esta noche.
English: I can go to the restaurant tonight.
Targets:
  - puedo
CompetingTargetForms:
  - podemos

## phrase: poder-02

Spanish: Podemos hacer una reserva para mañana.
English: We can make a reservation for tomorrow.
Targets:
  - podemos
CompetingTargetForms:
  - puedo

## phrase: poder-03

Spanish: Puedo comprar algo para la cena.
English: I can buy something for dinner.
Targets:
  - puedo
CompetingTargetForms:
  - podemos

## phrase: poder-04

Spanish: Podemos ir al hotel después del almuerzo.
English: We can go to the hotel after lunch.
Targets:
  - podemos
CompetingTargetForms:
  - puedo

## phrase: poder-05

Spanish: Puedo llamar al hotel esta mañana.
English: I can call the hotel this morning.
Targets:
  - puedo
CompetingTargetForms:
  - podemos

## phrase: poder-06

Spanish: Podemos salir temprano mañana.
English: We can leave early tomorrow.
Targets:
  - podemos
CompetingTargetForms:
  - puedo

# Stages

## stage: spanish-easy

PromptLanguage: spanish
Difficulty: easy
Phrases:
  - poder-01
  - poder-02

## stage: spanish-medium

PromptLanguage: spanish
Difficulty: medium
Phrases:
  - poder-01
  - poder-02
Masks:
  poder-01:
    - puedo
    - ir
  poder-02:
    - podemos
    - reserva

## stage: spanish-hard

PromptLanguage: spanish
Difficulty: hard
Phrases:
  - poder-01
  - poder-02

## stage: english-easy

PromptLanguage: english
Difficulty: easy
Phrases:
  - poder-01
  - poder-02

## stage: english-medium

PromptLanguage: english
Difficulty: medium
Phrases:
  - poder-01
  - poder-02
Masks:
  poder-01:
    - puedo
    - ir
  poder-02:
    - podemos
    - reserva

## stage: english-hard

PromptLanguage: english
Difficulty: hard
Phrases:
  - poder-01
  - poder-02
