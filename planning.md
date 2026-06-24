# TakeMeter Planning

## Classification Task

Classify CU Boulder student discussion posts into one of four categories:

- Question
- Advice
- Experience
- Opinion

CU Boulder discussions are a good fit for this task because students frequently ask questions, share experiences, provide recommendations, and express opinions about campus life.


## Label Definitions

### Question

The post is asking for information, recommendations, or help.

Example:

"What are the best dorms for freshmen at CU Boulder?"

### Advice

The post is giving guidance or recommending an action.

Example:

"Register for classes as soon as possible."

### Experience

The post is describing something personally experienced by the author.

Example:

"I transferred to CU Boulder during my sophomore year."

### Opinion

The post is expressing a judgment, complaint, preference, or reaction.

Example:

"Parking permits are ridiculously expensive."

## Ambiguous Example

Example:

"Parking permits are a waste of money. Just take the bus."

Possible labels:
- Opinion
- Advice

Decision rule:

Label according to the primary purpose of the statement. If the statement mainly expresses a judgment, classify it as Opinion. If the statement mainly recommends an action, classify it as Advice.

## Expected Challenges

- Distinguishing Experience from Opinion.
- Distinguishing Advice from Opinion.
- Short posts with limited context.

## Data Collection Plan

The dataset will contain at least 200 examples covering common CU Boulder discussion topics such as housing, transportation, study spaces, dining, student organizations, registration, and campus life.

Examples will be labeled according to the four-category taxonomy:

* Question
* Advice
* Experience
* Opinion

The goal is to maintain a roughly balanced distribution across labels to reduce class imbalance.

## Evaluation Metrics

The primary evaluation metric will be accuracy on a held-out test set.

Additional metrics will include:

* Precision
* Recall
* F1-score
* Confusion matrix analysis

These metrics were chosen because they provide insight into both overall performance and label-specific performance.

## Success Threshold

A model will be considered "good enough" if it achieves at least 70% accuracy on the test set while maintaining reasonable performance across all four labels.

Accuracy alone is not sufficient; the model should also avoid consistently collapsing one label into another.

## AI Tool Plan

AI tools may be used to:

* Brainstorm and refine label definitions.
* Generate candidate examples for review.
* Analyze model failure patterns and confusing examples.

All labels and final dataset decisions will be reviewed manually before inclusion in the dataset.
