# Video Annotation Guidelines

## Annotation Task
Pedestrian detection and multi-object tracking using bounding boxes.

## Annotation Tool
Label Studio.

## Annotation Category

**Person:** Any clearly identifiable human pedestrian appearing in the video.

## Annotation Instructions

1. Review the video before beginning annotation.
2. Identify clearly visible pedestrians.
3. Draw bounding boxes around the visible bodies of pedestrians.
4. Assign a unique tracking identity to each individual.
5. Maintain consistent tracking identities as people move through the video.
6. Adjust bounding boxes to follow changes in pedestrian positions.
7. Handle temporary occlusions without unnecessarily creating new identities.

## Annotation Rules

- Annotate eligible pedestrians throughout the video.
- Do not annotate people appearing on posters, billboards, or screens.
- Do not assign a new identity to an already tracked person.
- Maintain existing identities when pedestrians are temporarily obscured.
- Do not guess when a pedestrian cannot be clearly identified.
- Ensure bounding boxes accurately cover visible body regions.

## Quality Control

Annotations should be reviewed for:

- Correct pedestrian identification.
- Accurate bounding-box placement.
- Consistent tracking identities.
- Duplicate or missing annotations.
- Consistent application of annotation rules.

## Export Format
JSON (Label Studio annotation export).
