# Named Entity Recognition (NER) – News Articles

## Project Overview

This project demonstrates practical experience in text annotation through Named Entity Recognition (NER).

The task involved identifying and classifying named entities in 10 news-style documents using Doccano. Each identified entity was assigned an appropriate label based on predefined annotation guidelines.

## Project Objectives

- Identify named entities in unstructured text.
- Classify entities into predefined categories.
- Apply consistent annotation rules.
- Maintain accurate entity boundaries.
- Perform quality checks on the completed dataset.

## Tools Used

- **Doccano:** Text annotation and dataset export.
- **JSONL:** Storage format for annotated data.
- **GitHub:** Project documentation and version control.

## Annotation Categories

Six entity categories were used:

| Label | Description |
|---|---|
| PERSON | Names of individuals. |
| ORGANIZATION | Companies, institutions and formal organizations. |
| LOCATION | Geographical places. |
| DATE | Calendar dates and date expressions. |
| PRODUCT | Named products and branded offerings. |
| EVENT | Named events, conferences and festivals. |

## Dataset Information

| Metric | Result |
|---|---|
| Number of documents | 10 |
| Total entity annotations | 41 |
| Number of entity categories | 6 |
| Annotation tool | Doccano |
| Export format | JSONL |

## Project Workflow

1. Created a sequence-labeling project in Doccano.
2. Defined six entity categories.
3. Imported 10 news-style text documents.
4. Annotated the documents according to the project guidelines.
5. Exported the completed annotations in JSONL format.
6. Reviewed the exported dataset for missing entities, incorrect labels, boundary errors and overlapping spans.
7. Corrected identified issues and documented the quality checks.

## Project Files

| File | Description |
|---|---|
| `NER_Annotation_Guidelines.md` | Rules and instructions used for annotation. |
| `ner_dataset.jsonl` | The completed annotated dataset. |
| `QA_Report.md` | Quality assurance checks and corrections. |

## Skills Demonstrated

- Text annotation
- Named Entity Recognition
- Entity classification
- Character-span identification
- Annotation guideline development
- Dataset quality assurance
- JSONL data handling
- Doccano

## Conclusion

This project provided practical experience in identifying, classifying and reviewing named entities in text data. It demonstrates an understanding of annotation workflows, consistency, entity boundaries and basic data quality assurance.
