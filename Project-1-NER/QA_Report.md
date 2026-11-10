# Quality Assurance Report
## Named Entity Recognition (NER) – News Articles

### 1. Project Summary

This report documents the quality review conducted on the Named Entity Recognition dataset created using Doccano.

| Item | Details |
|---|---|
| Project | Named Entity Recognition – News Articles |
| Annotation tool | Doccano |
| Dataset size | 10 documents |
| Total annotations | 41 |
| Annotation categories | 6 |
| Export format | JSONL |

### 2. Quality Checks Performed

The exported annotations were manually reviewed using the following criteria:

- **Entity completeness:** Checked whether relevant named entities had been identified.
- **Label accuracy:** Verified that each entity was assigned the appropriate category.
- **Span accuracy:** Checked that the highlighted text matched the complete entity name.
- **Punctuation:** Checked that unnecessary punctuation and surrounding spaces were excluded.
- **Consistency:** Reviewed similar entities to ensure that annotation rules were applied consistently.
- **Overlapping annotations:** Checked for inappropriate overlapping entity spans.

### 3. Errors Identified and Corrections Made

During the review, the following issues were identified:

| Document ID | Issue identified | Correction |
|---|---|---|
| 146 | The PERSON span included an unnecessary title and had an incorrect starting boundary. | Corrected the span to cover only "Amina Bello". |
| 152 | The organization "United Nations" was missing. | Added the ORGANIZATION annotation. |
| 153 | The ORGANIZATION span did not cover the complete university name. | Corrected it to cover "University of Ibadan". |
| 153 | The LOCATION annotation for "Ibadan" overlapped with the university name. | Removed the overlapping annotation. |
| 153 | The LOCATION span for "Nigeria" had an incorrect starting boundary. | Corrected the span to cover only "Nigeria". |

### 4. Final Review Results

After the corrections, the dataset was reviewed again.

The final exported dataset contains:

- 10 text documents.
- 41 entity annotations.
- 6 entity categories.
- No identified overlapping spans.
- Corrected entity boundaries and labels based on the annotation guidelines.

### 5. Conclusion

The quality assurance process helped identify and correct missing entities, inaccurate character boundaries, and overlapping annotations.

The final dataset was reviewed for consistency and is ready to serve as a practical NER portfolio project.

**Note:** This review was a manual quality check. An independent second-annotator review and inter-annotator agreement assessment were not conducted.
