# Probabilistic Language Models

- [Probabilistic Language Models](#probabilistic-language-models)
  - [Introduction](#introduction)
  - [Results](#results)
  - [Sources](#sources)

## Introduction

A popular idea in computational linguistics is to create a probabilistic model of language.  Such a model assigns a probability to every sentence in English in such a way that more likely sentences (in some sense) get higher probability.  If you are unsure between two possible sentences, pick the higher probability one.

Some models:

-  `unigram`: words generated one at a time, drawn from a fixed distribution.
-  `bigram`: probability of word depends on previous word.
- `trigram`: probability of the word depends of previous two words.

This repository contains a notebook that trains unigram, bigram, and trigram probabilistic language models on the Universal Declaration of Human Rights corpus in the following languages - English, French, Italian, and Spanish.

The models are then used, in pairs, to try and predict the language of a previously unseen body of text from the same document.

## Results

```
*******TEST SETS*********


Accuracy: English vs French

Unigram: = 78.20000
Bigram: = 91.80000
Trigram: = 99.00000


Accuracy: Spanish vs Italian

Unigram: = 67.00000
Bigram: = 84.80000
Trigram: = 96.30000
```

## Sources

- Guangwei Yuan's lecture notes for Dynamic Programming: Segmentation (1999)