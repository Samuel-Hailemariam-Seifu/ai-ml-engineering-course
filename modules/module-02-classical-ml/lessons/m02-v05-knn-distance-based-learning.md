# k-Nearest Neighbors (k-NN)
## Learning by Remembering and Measuring Distance

---

## Why k-NN Is Important

k-Nearest Neighbors looks almost too simple.

There is:
- No training phase
- No weights to learn
- No optimization loop

And yet, it can perform surprisingly well.

This forces us to rethink:
> what “learning” really means.

---

## How k-NN Works (Conceptually)

k-NN follows a simple idea:

1. Store all training data
2. For a new input:
   - find the closest points
   - look at their labels
3. Predict based on neighbors

That’s it.

No parameter updates.
No gradient descent.

---

## Distance Is the Model

In k-NN:
- distance defines similarity
- similarity defines neighbors
- neighbors define predictions

If distance is poorly chosen,
the model fails.

k-NN is only as good
as its distance metric.

---

## k Controls Model Behavior

The parameter **k** controls complexity.

Small k:
- very flexible
- sensitive to noise
- jagged decision boundaries

Large k:
- smoother boundaries
- more bias
- less variance

k is a capacity control knob.

---

## Decision Boundaries in k-NN

k-NN creates boundaries that:
- follow data closely
- bend around points
- adapt to local structure

This makes k-NN:
- powerful with clean data
- fragile with noisy data

Geometry is everything.

---

## Feature Scaling Matters (A Lot)

Because k-NN uses distance:

- large-scale features dominate
- small-scale features are ignored

Without normalization:
- distance becomes meaningless
- predictions become arbitrary

This is why preprocessing is critical.

---

## k-NN and the Curse of Dimensionality

In high dimensions:
- all points become far apart
- distances lose meaning
- neighbors stop being “near”

This is called the **curse of dimensionality**.

k-NN struggles badly here.

---

## When k-NN Works Well

k-NN works best when:
- data is low-dimensional
- features are meaningful
- local similarity matters
- dataset size is moderate

It is often a strong baseline.

---

## When k-NN Is a Bad Choice

k-NN is a poor choice when:
- data is very large
- latency matters
- dimensions are high
- features are noisy

It trades computation at training
for computation at prediction.

---

## What k-NN Teaches Us

k-NN teaches an important lesson:

> Learning can mean storing data  
> and defining similarity correctly.

Not all models learn by optimization.

---

## The Big Takeaway

**Remember this:**

| Concept | Insight |
|:--------|:--------|
| k-NN | Learns by memory |
| Distance | Defines behavior |
| k | Controls complexity |
| Preprocessing | Is essential |

> This model makes geometry impossible to ignore.

---

## What’s Next

**Next video:**  
### *Decision Trees: Learning Rules from Data*

We’ll move from geometry
to rule-based learning.
