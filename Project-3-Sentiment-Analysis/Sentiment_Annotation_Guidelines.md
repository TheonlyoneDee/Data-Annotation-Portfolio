# Sentiment Analysis Annotation Guidelines

## 1. Introduction

These guidelines define the procedures and criteria used to classify text samples according to their expressed sentiment.

The purpose is to ensure consistency, accuracy, and reliability throughout the annotation process.

The annotation task uses document-level text classification, where each complete text sample receives one sentiment label.

## 2. Annotation Objectives

The objectives are to:

- Identify the overall sentiment expressed in a text.
- Distinguish between positive, negative, and neutral expressions.
- Apply consistent labeling criteria.
- Handle mixed sentiments and ambiguous expressions.
- Maintain annotation quality and consistency.

## 3. Label Definitions

Three sentiment labels are used in this project.

| Label | Definition |
|---|---|
| Positive | Text expressing satisfaction, happiness, approval, appreciation, or favourable experiences. |
| Negative | Text expressing dissatisfaction, disappointment, frustration, criticism, or unfavourable experiences. |
| Neutral | Text presenting factual information without a clearly expressed positive or negative opinion. |

## 4. Annotation Rules

### 4.1 Positive Sentiment

Assign POSITIVE when the text communicates a favourable opinion or experience.

Examples:
- The food was delicious.
- I love the quality of this product.
- The customer service was excellent.

### 4.2 Negative Sentiment

Assign NEGATIVE when the text communicates an unfavourable opinion or experience.

Examples:
- The delivery was extremely slow.
- I regret purchasing this product.
- The customer service was disappointing.

### 4.3 Neutral Sentiment

Assign NEUTRAL when the text provides information without expressing a clear positive or negative opinion.

Examples:
- The meeting starts at 10 a.m.
- I purchased two pairs of shoes.
- The restaurant is located in Lagos.

## 5. Handling Difficult Cases

### 5.1 Mixed Sentiment

Some texts contain both positive and negative expressions.

Example:

"The food was delicious, but the delivery was extremely slow."

Annotation: NEGATIVE.

Decision rule: Consider the overall message and identify the dominant sentiment. Where neither sentiment clearly dominates, use the context and main evaluative emphasis to make a consistent decision.

### 5.2 Sarcasm

Sarcasm occurs when words communicate a meaning different from their literal interpretation.

Example:

"What a fantastic product! The battery lasts barely two hours."

Annotation: NEGATIVE.

Decision rule: Interpret the intended meaning rather than relying on individual positive or negative words.

### 5.3 Ambiguous Expressions

Some statements suggest a possible problem without clearly expressing dissatisfaction.

Example:

"The washing machine makes an unusual noise during operation."

Annotation: NEGATIVE in this dataset because the unusual noise is presented as a potential product problem.

Decision rule: Where context is insufficient, annotators should avoid assuming an emotion that is not clearly supported by the text. Ambiguous cases should be flagged for review.

### 5.4 Neutral Statements

A factual statement should remain neutral even when it discusses a product or service.

Example:

"The restaurant offers indoor and outdoor seating."

Annotation: NEUTRAL.

## 6. Annotation Procedure

The following procedure was used:

1. Open the text document in Doccano.
2. Read the complete text.
3. Identify the overall sentiment.
4. Select the appropriate classification label.
5. Save the annotation.
6. Review completed annotations for consistency.

## 7. Quality Control Guidelines

The following checks should be performed:

- Every document must contain a text entry.
- Every document must have exactly one sentiment label.
- Labels must belong to the approved classification categories.
- Ambiguous and mixed-sentiment examples should receive additional review.
- The original text must remain unchanged.
- Annotation decisions should follow the documented guidelines.

## 8. Annotation Tools

| Tool | Purpose |
|---|---|
| Doccano | Text classification and annotation |
| GitHub | Project documentation and version control |
| JSONL | Dataset storage and export format |

## 9. Conclusion

These guidelines establish a consistent framework for sentiment classification.

Following the defined labeling criteria helps improve annotation quality and produces structured data suitable for natural language processing applications.
