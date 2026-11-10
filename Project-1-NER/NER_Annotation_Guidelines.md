# Named Entity Recognition (NER) Annotation Guidelines

## 1. Project Overview

**Project title:** Named Entity Recognition (NER) – News Articles  
**Task type:** Sequence Labelling  
**Annotation tool:** Doccano  
**Dataset size:** 10 text documents  
**Total annotations:** 41  

### Project Description

This project focuses on identifying and classifying named entities in news-style text. The objective is to accurately locate important entities such as people, organizations, locations, dates, products, and events.

The annotations can be used to support the development and evaluation of Natural Language Processing (NLP) systems, particularly Named Entity Recognition models.

## 2. Annotation Objectives

Annotators are expected to:

- Identify relevant named entities in each document.
- Assign the correct entity label.
- Highlight only the exact text representing the entity.
- Maintain consistent annotation decisions across all documents.
- Avoid including unnecessary words, spaces, or punctuation in entity spans.

## 3. Entity Categories and Definitions

The project uses six entity categories.

| Label | Definition | Example |
|---|---|---|
| PERSON | Names of individuals. | Amina Bello |
| ORGANIZATION | Names of companies, institutions, government bodies, and formal organizations. | African Development Bank |
| LOCATION | Names of geographical places, including cities, countries, and regions. | Abuja |
| DATE | Specific calendar dates and date expressions. | 12 March 2025 |
| PRODUCT | Names of identifiable products, services, or branded offerings. | SwiftPay |
| EVENT | Names of identifiable events, conferences, festivals, and forums. | Global Climate Summit |

## 4. General Annotation Rules

### Rule 1: Annotate the Exact Entity

Select only the words that form the named entity.

Correct: `Amina Bello`  
Incorrect: `President Amina Bello`

Titles and descriptive words should not be included unless they form part of the official entity name.

### Rule 2: Exclude Unnecessary Punctuation

Do not include commas, full stops, or other surrounding punctuation in an entity span.

Correct: `8 June 2025`  
Incorrect: `8 June 2025.`

### Rule 3: Do Not Annotate Ordinary Descriptions as Entities

Not every noun or descriptive phrase is a named entity.

For example, in the sentence:

"The government announced a new education programme."

The phrases "government" and "education programme" should not automatically receive entity labels because they are not specific named entities in this context.

### Rule 4: Use the Most Appropriate Label

Each entity should receive the label that best represents its identity.

For example:
- Apple — ORGANIZATION
- iPhone 17 — PRODUCT
- California — LOCATION

### Rule 5: Avoid Overlapping Annotations

When one named entity contains another word that could independently qualify as an entity, annotate the complete entity rather than creating overlapping spans.

Example:

`University of Ibadan`

Annotate the complete name as ORGANIZATION rather than separately annotating "Ibadan" as LOCATION within the same span.

### Rule 6: Maintain Consistency

Similar entities should be annotated using the same rules throughout the dataset.

## 5. Annotation Procedure

The following procedure was used when annotating the dataset:

1. Open the NER project in Doccano.
2. Read each document carefully.
3. Identify all relevant named entities.
4. Highlight each entity.
5. Assign the appropriate label.
6. Review the highlighted text to ensure that the boundaries are accurate.
7. Submit the annotation and proceed to the next document.
8. Review completed annotations before exporting the dataset.

## 6. Quality Assurance Guidelines

After annotation, the dataset should be reviewed for the following issues:

- **Entity omission:** Relevant named entities that were not annotated.
- **Incorrect classification:** An entity assigned to the wrong category.
- **Boundary errors:** Extra or missing characters in an annotated span.
- **Punctuation errors:** Unnecessary punctuation included in an entity.
- **Inconsistency:** Similar entities treated differently across documents.
- **Overlapping spans:** Entity annotations that improperly overlap.

The exported dataset was reviewed to identify and correct annotation errors before final submission.

## 7. Dataset Format

The annotated dataset was exported in JSONL (JSON Lines) format.

Each record contains:

- `id`: Unique document identifier.
- `text`: Original text.
- `label`: List of annotated entity spans and their corresponding labels.
- `Comments`: Additional annotation comments, where applicable.

The entity spans use character offsets, with the starting position included and the ending position excluded.

## 8. Expected Outcome

The expected outcome is a consistently annotated news-text dataset containing correctly identified and classified named entities.

The completed dataset serves as a practical demonstration of text annotation, entity recognition, annotation consistency, and basic data quality assurance.
