# TakeMeter Planning

## Classification Task

Classify CU Boulder student discussion posts into one of four categories:

- Question
- Advice
- Experience
- Opinion

## Label Definitions

### Question

The post is asking for information, recommendations, or help.

### Advice

The post is giving guidance or recommending an action.

### Experience

The post is describing something personally experienced by the author.

### Opinion

The post is expressing a judgment, complaint, preference, or reaction.

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