# Matrix Multiplication
## How Models Transform Data

---

## Why Matrix Multiplication Matters

If vectors represent data,  
then **matrix multiplication** is how models **transform** that data.

Almost every ML model can be described as:

> input vectors → matrix transformations → output vectors

> This is not a coincidence.  
> This is the core mechanism.

---

## The Right Mental Model

> Forget the multiplication rules for now.

Think of a matrix as:
- a **machine**
- a **transformation**
- a **set of directions**

Matrix multiplication means:

> “Apply this transformation to the data.”

---

## From Dot Product to Matrices

Earlier, we saw that:
- A dot product compares two vectors.

Matrix multiplication is just:
- **many dot products at once**

Each row of a matrix:
- computes one dot product
- extracts one learned pattern

> This is how models scale from **one feature**  
> to **thousands**.

---

## What a Matrix Represents in ML

In machine learning, a matrix often represents:

- Model parameters (weights)
- Learned features
- Transformations between spaces

When you multiply:
- data matrix × weight matrix

> You are applying **learned structure** to data.

---

## Data as a Matrix

Most datasets are matrices.

| Part | Meaning |
|:-----|:--------|
| Rows | Data points |
| Columns | Features |

**Example:**
- 10,000 samples  
- 100 features each

> That is a **10,000 × 100 matrix**.

Matrix multiplication lets us:
- process all samples at once
- leverage hardware efficiently
- reason about models cleanly

---

## Linear Layers Are Matrix Multiplications

A linear layer in a neural network does:

> output = input × weights + bias

**Conceptually:**
- input vectors are transformed
- new representations are created
- information is re-expressed

> Nothing mystical is happening.  
> It’s structured geometry.

---

## Transformation, Not Calculation

**This is important:**

Matrix multiplication is not just arithmetic.  
It is **geometric transformation**.

It can:
- rotate data
- scale dimensions
- stretch or compress space
- reorient representations

> Models learn which transformations are useful.

---

## Why Order Matters

Matrix multiplication is **not commutative**.

This means:
- A × B ≠ B × A

In ML terms:
- the order of layers matters
- the sequence of transformations matters

> Changing order changes meaning.

---

## Stacking Transformations

Deep learning works by:

- applying one transformation
- then another
- then another

Each layer:
- reshapes the data
- highlights different patterns

> Depth comes from **composition**, not complexity.

---

## Where Non-Linearity Fits

Without non-linearity:
- stacked linear transformations collapse into one

Non-linearities:
- bend space
- introduce complexity
- make learning powerful

> But the backbone remains linear algebra.

---

## The Big Takeaway

**Remember this:**

| Concept | Role |
|:--------|:-----|
| Vectors | Represent data |
| Dot products | Measure alignment |
| Matrices | Apply transformations |
| Layers | Stack transformations |

> Machine learning is linear algebra  \n> plus a small amount of controlled non-linearity.

---

## What’s Next

>**Next video:**  
>### *Eigenvectors, Eigenvalues, and Why PCA Works*

We’ll see how certain directions
carry more information than others.
