# Train / Validation / Test Splits
## Avoiding Data Leakage

---

## Why This Video Matters

Many ML models look impressive
but fail in the real world.

Often, the reason is not the model —
it’s **data leakage**.

Leakage creates false confidence
and broken systems.

---

## The Purpose of Splitting Data

We split data to answer one question:

> “How will this model perform on unseen data?”

If the answer is contaminated,
the evaluation is meaningless.

---

## The Three Roles of Data

**A clean ML workflow uses three sets:**

| **Dataset** | **Purpose** |
|:------------|:------------|
| **Training set** | Fit model parameters |
| **Validation set** | Tune hyperparameters<br>Choose models |
| **Test set** | Final evaluation (once) |

> Each set has a strict role.

---

## What Data Leakage Is

Data leakage happens when:
- information from outside the training set
- influences model training

This can happen directly or indirectly.

Leakage is subtle —
and very common.

---

## Common Leakage Patterns

**Some frequent causes:**
- Scaling or encoding before splitting
- Using future information
- Target leakage in features
- Reusing test data during tuning
- Time-based data shuffled incorrectly

> These errors produce unrealistically good results.

---

## Why Leakage Is Dangerous

**Leakage:**
- Inflates metrics
- Hides generalization problems
- Passes internal tests
- Fails in production

> The model appears smart —  
> until it meets reality.

---

## Proper Splitting Order

Always follow this order:

1. Split data first
2. Fit preprocessing on training data only
3. Apply preprocessing to validation/test

Never reverse this order.

Pipelines exist to enforce this.

---

## Special Case: Time-Series Data

For time-based data:
- random splitting is wrong
- future information leaks backward

Correct approach:
- train on past
- validate on future
- test on later future

Time defines reality.

---

## Validation Is for Decisions

Use validation data to:
- choose hyperparameters
- compare models
- decide when to stop training

Once you look at test performance,
the test set is no longer clean.

---

## One Test Set Rule

You should evaluate on the test set:
> **once**

If you evaluate repeatedly,
you are training on it indirectly.

This is silent leakage.

---

## Cross-Validation (Preview)

Cross-validation:
- reduces variance
- uses data efficiently

But it must still:
- respect data boundaries
- avoid leakage
- reflect real-world usage

We’ll cover this properly soon.

---

## How to Detect Leakage

Red flags:
- unusually high accuracy
- performance drops sharply in production
- test results too stable across experiments

When results look too good,
they usually are.

---

## The Big Takeaway

**Remember this:**

| **Principle** | **Insight** |
|:--------------|:------------|
| **Splitting** | Defines evaluation truth |
| **Leakage** | Invalidates results |
| **Order** | Matters |
| **Pipelines** | Protect you |

> A leaky evaluation  
> is worse than no evaluation.

---

---

## What's Next

> **Next video:**  
> ### *Preprocessing with Pipelines (Reproducible ML)*

We'll show how pipelines  
prevent leakage by design.
