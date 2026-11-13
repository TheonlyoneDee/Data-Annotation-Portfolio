# Quality Assurance Report – POS Tagging Project

## 1. Project Summary

This project involved Part-of-Speech (POS) tagging of 50 English sentences using the Universal Dependencies Part-of-Speech (UPOS) tag set.

Each word was assigned a grammatical category based on its function and context within the sentence.

## 2. Quality Checks Performed

The following checks were carried out:

- **Dataset completeness:** Confirmed that all 50 sentences were included.
- **Annotation completeness:** Checked that every sentence had POS annotations.
- **Label consistency:** Reviewed the annotations to ensure that the correct UPOS labels were used consistently.
- **Token boundaries:** Checked that annotation spans matched the intended words and punctuation.
- **Overlapping annotations:** Checked for unintended overlapping spans.
- **Punctuation:** Verified that punctuation marks were appropriately tagged.
- **Contextual accuracy:** Reviewed words whose grammatical roles depend on how they are used in a sentence.

## 3. Common Annotation Considerations

Special attention was given to:

- Distinguishing determiners from pronouns.
- Identifying auxiliary verbs.
- Differentiating adverbs from adjectives.
- Correctly tagging particles such as "not" and infinitive "to".
- Identifying proper nouns and unknown or unclassified tokens.

## 4. Quality Assurance Results

The final dataset contains 50 annotated sentences.

The review found no missing annotations, invalid spans, unintended overlapping annotations, or uncovered characters.

The annotations were also reviewed for consistency with the project's guidelines and UPOS tagging conventions.

## 5. Conclusion

The POS tagging dataset passed the quality checks performed during this project.

This project demonstrates practical experience in text annotation, grammatical classification, annotation guidelines, and basic dataset quality assurance.
