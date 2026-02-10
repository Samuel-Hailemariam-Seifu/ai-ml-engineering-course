# Decision Boundaries and Model Capacity
## How Models Carve Up Space

---

## Why This Video Matters

So far, you’ve seen:
- Linear regression
- Logistic regression

Both rely on **simple, linear boundaries**.

But real-world data is rarely that simple.

This video explains:
> why different models behave differently  
> and what “model complexity” actually means.

---

## Decision Boundaries Revisited

A **decision boundary** separates:
- one class from another
- one region of space from another

Every classifier:
- draws boundaries
- partitions space
- assigns labels to regions

Different models draw **different shapes**.

---

## Linear Models: Simple Boundaries

Linear models create:
- straight lines (2D)
- planes (3D)
- hyperplanes (higher dimensions)

Advantages:
- easy to understand
- stable
- fast
- generalize well

Limitations:
- cannot bend
- cannot capture complex patterns

---

## Nonlinear Boundaries (Intuition)

More flexible models can:
- curve boundaries
- create pockets
- separate complex structures

This flexibility allows:
- better fit to data
- higher training performance

But it comes at a cost.

---

## Model Capacity (Core Concept)

**Model capacity** describes:
> how complex a function a model can represent

Low capacity:
- simple boundaries
- limited flexibility
- risk of underfitting

High capacity:
- complex boundaries
- many degrees of freedom
- risk of overfitting

Capacity is not good or bad by itself.

---

## Capacity vs Data

Capacity must match:
- data complexity
- data size
- noise level

High capacity + little data → overfitting  
Low capacity + complex data → underfitting  

This mismatch causes most failures.

---

## Visualizing Capacity (Mental Model)

Imagine drawing boundaries by hand:

- straight ruler → low capacity
- bendable wire → medium capacity
- freehand drawing → high capacity

More freedom means:
- more expressive power
- more ways to be wrong

---

## Why “More Complex” Isn’t Always Better

High-capacity models:
- fit noise easily
- memorize training data
- behave unpredictably on new data

Good ML is not about:
> fitting the data perfectly

It’s about:
> fitting the **right structure**

---

## Regularization as Capacity Control

Regularization:
- restricts boundary complexity
- smooths decision regions
- improves generalization

It’s how engineers
tame powerful models.

---

## Every Algorithm Is a Boundary Designer

Think of algorithms this way:

- linear models → straight boundaries
- k-NN → very jagged boundaries
- trees → box-like boundaries
- ensembles → smoother, flexible boundaries

This lens unifies everything.

---

## The Big Takeaway

**Remember this:**

| Concept | Insight |
|:--------|:--------|
| Classifiers | Carve up space |
| Boundaries | Define behavior |
| Capacity | Controls flexibility |
| Generalization | Depends on balance |

> If you understand boundaries,  
> you understand classification.

---

## What’s Next

**Next video:**  
### *k-Nearest Neighbors (k-NN) and Distance-Based Learning*

We’ll explore a model
that learns almost nothing —
and yet can be very powerful.
