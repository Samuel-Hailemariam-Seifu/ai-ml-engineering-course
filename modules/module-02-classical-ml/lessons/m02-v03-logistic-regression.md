# Logistic Regression
## Classification as Geometry

---

## Why Logistic Regression Matters

Logistic regression is often misunderstood.

People think:
- It’s about probabilities
- It’s about a sigmoid function
- It’s about classification formulas

In reality, logistic regression is about:

> **Separating space with a decision boundary**

> Once you see that, everything clicks.

---

## From Regression to Classification

| **Task Type** | **Output** |
|:--------------|:-----------|
| **Linear regression** | A continuous number |
| **Classification** | A category<br>A yes / no decision |

**But the learning loop is the same:**
- Model
- Loss
- Optimization
- Generalization

> Only the interpretation changes.

---

## The Model Is Still Linear

Logistic regression uses:
- input vector
- weight vector
- dot product

Just like linear regression.

The difference is **how we interpret the output**.

---

## Decision Boundary (Core Idea)

The dot product produces a score.

Logistic regression asks:
> On which side of a boundary does this point lie?

That boundary is:
- a line in 2D
- a plane in 3D
- a hyperplane in higher dimensions

Classification = space partitioning.

---

## Geometry, Not Probability (Important)

The model does NOT think in probabilities.

It thinks in:
- alignment
- direction
- distance from the boundary

Probability is just a **convenient mapping**
for humans to interpret confidence.

---

## Why the Sigmoid Exists

The sigmoid function:
- squashes scores into a fixed range
- makes outputs interpretable
- supports smooth optimization

It does NOT make the model smarter.

The intelligence is in the boundary.

---

## Loss Function Shapes the Boundary

The loss function:
- penalizes confident wrong predictions
- rewards confident correct ones

This pushes the boundary:
- away from ambiguous regions
- toward clearer separation

Loss defines geometry.

---

## Linear Separability

Logistic regression works well when:
- classes are roughly separable
- a straight boundary is sufficient

It struggles when:
- data is highly nonlinear
- patterns are intertwined

This limitation is intentional and informative.

---

## Overconfidence and Regularization

Without regularization:
- the model can become overconfident
- weights can grow very large
- decision boundaries become unstable

Regularization keeps:
- boundaries smoother
- predictions more reliable

Geometry stays sane.

---

## Why Logistic Regression Is Still Used

Logistic regression is used because:
- it is interpretable
- it is fast
- it is stable
- it provides strong baselines

Many complex models
are judged against it.

---

## The Big Takeaway

**Remember this:**

| Concept | Insight |
|:--------|:--------|
| Classification | Separating space |
| Logistic regression | Learns a boundary |
| Loss | Shapes that boundary |
| Probability | Is just interpretation |

> If you understand the geometry,  
> classification stops being confusing.

---

---

## What's Next

> **Next video:**  
> ### *Decision Boundaries and Model Capacity*

We'll compare how different models  
carve up space differently.
