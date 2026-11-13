# POS Annotation Guidelines

## 1. Annotation Objective

The objective is to identify and classify every word in each sentence according to its grammatical role.

Punctuation marks are also annotated separately.

## 2. Tagging Standard

The project uses the 17 Universal POS (UPOS) tags.

| Tag | Meaning | Description |
|---|---|---|
| ADJ | Adjective | Describes a noun or pronoun. |
| ADP | Adposition | Expresses relationships such as location, direction, or time. |
| ADV | Adverb | Modifies a verb, adjective, or another adverb. |
| AUX | Auxiliary | Helps another verb express tense, mood, or grammatical meaning. |
| CCONJ | Coordinating Conjunction | Connects words, phrases, or clauses of equal grammatical status. |
| DET | Determiner | Introduces or specifies a noun. |
| INTJ | Interjection | Expresses emotion, reaction, or attention. |
| NOUN | Noun | Names a person, place, thing, or concept. |
| NUM | Numeral | Expresses a number or quantity. |
| PART | Particle | A grammatical particle that does not fit another category. |
| PRON | Pronoun | Replaces or refers to a noun phrase. |
| PROPN | Proper Noun | Names a specific person, place, organization, or entity. |
| PUNCT | Punctuation | Includes commas, periods, question marks, and other punctuation marks. |
| SCONJ | Subordinating Conjunction | Introduces a subordinate clause. |
| SYM | Symbol | Represents a symbol or special character. |
| VERB | Verb | Expresses an action, occurrence, or state. |
| X | Other | Used for tokens that cannot be confidently assigned another POS category. |

## 3. Annotation Rules

### 3.1 Word Identification
Each word in a sentence must receive an appropriate POS tag.

### 3.2 Punctuation
Punctuation marks are annotated separately using the PUNCT tag.

Examples include:
- Full stops.
- Commas.
- Question marks.
- Exclamation marks.

### 3.3 Proper Nouns
Specific names of people, places, and entities are tagged PROPN.

Examples:
- Michael
- Amina
- Abuja
- Kano

### 3.4 Determiners and Possessives
Words that introduce or specify nouns are tagged DET.

Examples:
- The
- A
- My
- Our
- Their
- His

### 3.5 Auxiliary Verbs
Helping verbs are tagged AUX.

Examples:
- Is
- Are
- Was
- Have
- Can
- Will
- Should

### 3.6 Particles
Grammatical particles are tagged PART.

Examples:
- Not
- Infinitive "to" when it appears before a verb.

### 3.7 Adjectives and Adverbs
Adjectives describe nouns, while adverbs modify verbs, adjectives, or other adverbs.

Examples:
- Beautiful — ADJ
- Carefully — ADV
- Quickly — ADV

### 3.8 Symbols and Unclassified Tokens
Symbols are tagged SYM, while tokens that cannot be confidently classified are tagged X.

Examples:
- #A17 — SYM
- qzx — X

## 4. Tokenization Approach

The project uses whitespace based word identification.

Each word is annotated according to its position in the original sentence. Punctuation is treated as a separate token where it is separated by the text.

For this project, possessive forms such as "patient's" remain attached to the word and are annotated as a single token.

## 5. Annotation Quality Standards

The following quality checks are applied:

- Every word must have an appropriate POS tag.
- Punctuation must be annotated.
- Character positions must match the original sentence.
- Annotations must not overlap.
- No word or punctuation mark should be unintentionally left unannotated.
- The same tagging conventions should be applied consistently throughout the dataset.

## 6. Dataset Information

- Project: English Part-of-Speech Tagging
- Dataset size: 50 sentences
- Annotation tool: Doccano
- Annotation type: Sequence Labeling
- Tagging standard: Universal Dependencies UPOS
- Language: English

## 7. Conclusion

This project demonstrates practical experience in grammatical text annotation, POS classification, sequence labeling, and annotation quality control.
