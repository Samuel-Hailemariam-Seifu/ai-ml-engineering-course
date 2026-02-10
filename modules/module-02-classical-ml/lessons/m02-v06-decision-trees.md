# Decision Trees
## Learning Rules from Data

---

## Why Decision Trees Matter

So far, we’ve seen models that:
- Measure alignment (linear, logistic)
- Measure distance (k-NN)

Decision trees are different.

They learn by:
> asking a sequence of simple questions.

This makes them:
- Intuitive
- Interpretable
- Very powerful

---

## The Core Idea

A decision tree works like this:

1. Ask a question about one feature
2. Split the data based on the answer
3. Repeat the process on each subset
4. Stop when predictions are clear enough

Each path becomes a **rule**.

---

## Thinking in If–Then Rules

A trained decision tree can be read as:

- IF feature A > threshold  
- AND feature B ≤ threshold  
- THEN predict class X

This rule-based nature is
what makes trees easy to interpret.

---

## How Trees Choose Questions

At each step, the tree asks:

> “Which question best separates the data?”

“Best” means:
- reduces uncertainty
- increases purity
- creates more homogeneous groups

Trees greedily choose
the best split **right now**.

---

## Greedy Does Not Mean Stupid

Trees are greedy:
- they don’t plan ahead
- they optimize locally

This works surprisingly well,
but it also explains some weaknesses.

Local decisions can lead to
globally suboptimal trees.

---

## Decision Boundaries of Trees

Trees create boundaries that are:
- axis-aligned
- box-like
- rectangular regions

They do not create smooth curves.

This gives trees:
- flexibility
- sharp decisions
- high variance

---

## Overfitting in Trees

Decision trees can easily:
- memorize training data
- grow very deep
- create tiny regions

A fully grown tree
almost always overfits.

Depth is capacity.

---

## Controlling Tree Complexity

We control trees by limiting:
- maximum depth
- minimum samples per leaf
- number of splits

These controls are
forms of regularization.

Without them, trees are unstable.

---

## Why Trees Are Unstable

Small changes in data can:
- change early splits
- completely reshape the tree

This instability is not a bug —
it explains why ensembles work so well.

---

## When Trees Work Well

Decision trees shine when:
- features are meaningful
- relationships are rule-based
- interpretability matters
- data has mixed types

They require little preprocessing.

---

## What Trees Teach Us

Trees teach an important lesson:

> Learning can be about discovering rules,
> not just fitting functions.

Different models learn in
fundamentally different ways.

---

## The Big Takeaway

**Remember this:**

| Concept | Insight |
|:--------|:--------|
| Trees | Learn by splitting |
| Splits | Create rules |
| Depth | Controls complexity |
| Interpretability | Comes naturally |

> Trees trade smoothness  
> for clarity.

---

---

## What's Next

> **Next video:**  
> ### *Ensembles: Why Many Weak Models Beat One Strong Model*

We'll see how trees become powerful  
when they work together.
