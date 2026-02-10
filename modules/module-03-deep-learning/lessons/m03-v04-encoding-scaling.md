# Encoding & Scaling Correctly
## Silent Bug Killers in Machine Learning

---

## Why This Video Matters

Some of the worst ML bugs:
- do not crash your code
- do not raise exceptions
- do not look wrong

They quietly destroy performance.

Most of these bugs come from:
> incorrect encoding and scaling.

---

## Models Only Understand Numbers

ML models do not understand:
- categories
- text
- meaning
- order (unless you give it)

They only understand numbers.

How you convert reality into numbers
changes how the model thinks.

---

## Categorical Features (The Trap)

Categorical features:
- country
- job title
- product type
- user segment

These are **labels**, not quantities.

If you encode them incorrectly,
you inject fake meaning.

---

## The Cardinality Mistake

Bad encoding example:
- “Engineer” = 1
- “Manager” = 2
- “CEO” = 3

This implies:
- CEO > Manager > Engineer

The model will believe this —
even though it’s nonsense.

---

## One-Hot Encoding (Safe Default)

One-hot encoding:
- removes fake ordering
- treats categories independently
- works well for many models

Trade-offs:
- increases dimensionality
- can become sparse

Still, it is the safest starting point.

---

## When Order Actually Matters

Sometimes categories are ordered:
- education level
- rating scales
- age groups

In these cases:
- ordinal encoding can make sense

The rule:
> only encode order if it exists in reality.

---

## Numerical Features and Scale

Numerical features can have very different ranges:
- age (0–100)
- income (0–100,000)
- clicks (0–10)

Many models are sensitive to scale.

If you ignore this:
- some features dominate
- others are ignored

---

## Which Models Care About Scaling

| **Scaling Sensitivity** | **Models** |
|:------------------------|:-----------|
| **Matters a lot** | Linear regression<br>Logistic regression<br>k-NN<br>SVMs<br>Neural networks |
| **Matters less** | Decision trees<br>Random forests<br>Gradient boosting |

> Knowing this saves time.

---

## Standardization vs Normalization

| **Approach** | **Method** | **Result** |
|:-------------|:-----------|:-----------|
| **Standardization** | Center to mean 0<br>Scale to unit variance | Mean = 0, Std = 1 |
| **Normalization** | Scale to fixed range | Range (e.g., 0–1) |

> There is no universal best choice.  
> Context and model matter.

---

## Scaling Must Be Fit on Training Data

This is critical:

> Never fit scalers on full data.

Always:
- fit scaler on training set
- apply to validation/test

Pipelines enforce this automatically.

Without pipelines,
this mistake is extremely common.

---

## Mixed Feature Types

Real datasets often have:
- numeric features
- categorical features
- missing values

Each type needs:
- different handling
- different transformers

Treating all features the same
is a design error.

---

## Encoding Changes Geometry

Remember:
- models carve up space
- distance and alignment matter

Encoding and scaling:
- reshape the space
- change distances
- change decision boundaries

You are changing the problem,
not just the inputs.

---

## Silent Failure Patterns

Warning signs:
- model performs worse than baseline
- coefficients look strange
- distance-based models behave randomly
- small feature changes cause big prediction swings

These often point to encoding/scaling issues.

---

## The Big Takeaway

**Remember this:**

| **Aspect** | **Impact** |
|:-----------|:-----------|
| **Encoding** | Injects meaning |
| **Scaling** | Controls influence |
| **Wrong choices** | Silently break models |
| **Pipelines** | Keep you safe |

> If results don't make sense,  
> check encoding and scaling first.

---

---

## What's Next

> **Next video:**  
> ### *Cross-Validation in Practice (Stable Model Evaluation)*

We'll show how to get  
reliable performance estimates.
