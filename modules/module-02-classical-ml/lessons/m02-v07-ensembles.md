# Ensembles
## Why Many Weak Models Beat One Strong Model

---

## Why Ensembles Matter

Decision trees are powerful,  
but they have a big weakness:

> they are unstable.

Small changes in data  
can produce very different trees.

Ensembles turn this weakness  
into a strength.

---

## The Core Idea

Instead of trusting one model:

> train many models  
> and combine their predictions

Each model makes mistakes.
But they don’t all make
the *same* mistakes.

Ensembles reduce error
by **averaging out failures**.

---

## Weak Models Can Be Strong Together

A **weak model**:
- slightly better than random
- imperfect
- limited on its own

When many weak models:
- see different data
- or focus on different errors

Their combination becomes strong.

This is the ensemble effect.

---

## Bagging (Bootstrap Aggregation)

Bagging works by:

1. Creating many random subsets of the data
2. Training one model on each subset
3. Averaging their predictions

Each model sees a slightly different world.

This reduces:
- variance
- overfitting
- sensitivity to noise

---

## Random Forests (Bagging + Randomness)

Random forests extend bagging by:

- using decision trees
- adding randomness in feature selection
- decorrelating trees

Each tree:
- is noisy
- is imperfect
- makes different mistakes

Together, they are robust.

---

## Why Random Forests Work So Well

Random forests succeed because:

- trees are high-variance models
- averaging reduces variance
- randomness prevents identical trees

This creates:
- strong generalization
- minimal tuning
- reliable baselines

That’s why they’re everywhere.

---

## Boosting (A Different Philosophy)

Boosting takes a different approach.

Instead of training models independently:

> train models sequentially  
> each new model focuses on previous mistakes

Errors get more attention over time.

---

## Boosting Intuition

Boosting asks:

- Which points are we getting wrong?
- How can we fix *those* specifically?

Over time:
- easy cases matter less
- hard cases matter more

This creates powerful models —
but also increases risk.

---

## Boosting Trade-offs

Boosting often achieves:
- very high accuracy
- strong performance on structured data

But it can:
- overfit noisy labels
- be sensitive to outliers
- require careful tuning

Power comes with responsibility.

---

## Bagging vs Boosting (Mental Model)

- Bagging:
  - reduces variance
  - stabilizes models
  - parallel training

- Boosting:
  - reduces bias
  - focuses on hard cases
  - sequential training

Different tools for different problems.

---

## Why Ensembles Dominate Classical ML

Ensembles work because:

- real data is noisy
- single models are brittle
- averaging improves reliability

Before deep learning,
ensembles were the state of the art.

They are still extremely competitive.

---

## The Big Takeaway

**Remember this:**

| Concept | Insight |
|:--------|:--------|
| Ensembles | Combine imperfect models |
| Diversity | More important than individual strength |
| Averaging | Reduces variance |
| Focusing on errors | Reduces bias |

> Many reasonable models  
> beat one perfect-looking model.

---

## What’s Next

**Next video:**  
### *Bias–Variance Trade-off*

We’ll explain why:
- some errors come from simplicity
- others come from complexity
