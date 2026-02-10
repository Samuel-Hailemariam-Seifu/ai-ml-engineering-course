# Linear Algebra for Machine Learning
## Intuition Before Math

---

## Why Linear Algebra Matters in ML

Most machine learning models are built on linear algebra.

Not because mathematicians like matrices,  
but because data, models, and transformations  
are naturally expressed as vectors and matrices.

> If you understand linear algebra,  
> models stop feeling mysterious.

---

## The Right Mental Model

> **Forget formulas for now.**

Think of linear algebra as the math of:
- **representing data**
- **transforming data**
- **comparing data**

> That's it.

---

## Vectors: Representing Information

A **vector** is just a list of numbers.

**In ML, vectors represent:**
- A data point
- A feature set
- An embedding
- Model parameters

**Examples:**
- A house → size, rooms, location
- A user → age, clicks, preferences
- A word → embedding values

> **One object → one vector.**

---

## Vectors Live in Space

You can imagine a vector as a point in space.

| **Vector Size** | **Space Dimension** |
|:----------------|:-------------------|
| 2 values | 2D space |
| 3 values | 3D space |
| 1000 values | High-dimensional space |

> Machine learning happens in these spaces.  
> **Distance and direction matter.**

---

## Distance Means Similarity

**In ML:**
- Close vectors → similar things
- Far vectors → different things

**Examples:**
- Similar users
- Similar images
- Similar words

> This is why distance metrics are everywhere.

---

## Matrices: Collections of Vectors

A **matrix** is just a collection of vectors.

**In practice:**
- **Rows** = data points
- **Columns** = features

**Example:**
- Dataset with 10,000 samples
- Each sample has 20 features

> That's a **10,000 × 20 matrix**.

---

## Models Are Matrix Operations

**Most models do the same thing:**

1. Take input vectors
2. Apply matrix operations
3. Produce output vectors

> Linear regression, neural networks,  
> and even transformers rely on this idea.

> **Different models → different transformations.**

---

## Linear Transformations (Big Idea)

**A linear transformation:**
- Rotates data
- Scales data
- Stretches data
- Compresses data

**But does NOT:**
- Bend space
- Create curves

> This is why linear models are limited —  
> and why we stack many layers.

---

## Why We Stack Layers

> One linear transformation is simple.

**Multiple linear transformations + non-linearities**  
can model complex patterns.

> This is the foundation of deep learning.  
> Linear algebra makes stacking possible.

---

## Dot Product: Measuring Alignment

**The dot product answers one question:**

> **How aligned are two vectors?**

**In ML, dot products are used for:**
- Similarity
- Scoring
- Attention mechanisms
- Predictions

> **High dot product → strong alignment.**

---

## This Shows Up Everywhere

**Linear algebra appears in:**
- Linear regression
- PCA
- Embeddings
- Neural networks
- Attention
- Optimization

> If you skip this,  
> everything later feels like memorization.

---

## What You Should Take Away

| **Do NOT Need** | **DO Need to Understand** |
|:----------------|:---------------------------|
| Memorize formulas yet | **Vectors represent things** |
| | **Matrices represent datasets and models** |
| | **Transformations change representations** |
| | **Distance and alignment drive decisions** |

> This intuition will carry you far.

---

---

## What's Next

> **Next video:**  
> ### *Vectors, Norms, and Distance*

We'll make similarity and distance  
feel completely natural.

> No heavy math — just clarity.
