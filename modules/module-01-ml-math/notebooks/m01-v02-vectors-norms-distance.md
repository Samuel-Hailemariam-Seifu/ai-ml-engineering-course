# Vectors, Norms, and Distance
## How ML Measures Similarity

---

## Why This Matters

Machine learning constantly asks questions like:

- Are these two users similar?
- Is this image close to that image?
- Does this input match what the model expects?

> All of these questions reduce to:  
> **How do we measure distance and similarity between vectors?**

---

## Vectors as Points in Space

A vector is not just a list of numbers.

**You can think of a vector as:**
- A point in space
- A direction
- A representation of something real

**Examples:**
- A document embedding
- A user profile
- A feature vector for one data point

> Machine learning operates in these spaces.

---

## Distance = Dissimilarity

**In ML:**
- Small distance → similar
- Large distance → different

**Distance is how models:**
- Cluster data
- Detect anomalies
- Compare embeddings
- Make decisions

> If distance is wrong,  
> everything built on top of it is wrong.

---

## Norms: Measuring Vector Size

A **norm** measures the size or length of a vector.

**Intuitively:**
> **"How big is this vector?"**

**Norms help us:**
- Compare magnitudes
- Normalize data
- Control optimization behavior

---

## The Most Common Norm: L2

The **L2 norm** is what people usually mean by "length".

**You can think of it as:**
- Straight-line distance from the origin
- Euclidean length

**Why it's popular:**
- Smooth
- Mathematically convenient
- Works well in practice

> Most ML models default to L2 behavior.

---

## Other Norms (Briefly)

> You don't need formulas yet — just intuition.

| **Norm** | **Characteristics** | **Use Cases** |
|:---------|:-------------------|:--------------|
| **L1 norm** | Sums absolute values<br>Encourages sparsity | Feature selection |
| **L∞ norm** | Looks at the largest value | Worst-case constraints |

> **Different norms → different behavior.**

---

## Distance Between Two Vectors

**Distance answers:**
> **"How far apart are these two points in space?"**

**Common choices:**
- Euclidean distance
- Manhattan distance
- Cosine distance

> Each one measures **difference differently**.  
> There is no universally correct choice.

---

## Cosine Similarity: Direction Matters

**Cosine similarity focuses on:**
- Direction
- Alignment

> It **ignores magnitude**.

**This is perfect for:**
- Text embeddings
- Semantic similarity
- Recommendation systems

> Two vectors can be far apart,  
> but still point in the same direction.

---

## Why Normalization Matters

**If features have very different scales:**
- Distance becomes meaningless
- Optimization becomes unstable
- Models behave unpredictably

**Normalization ensures:**
- Features contribute fairly
- Distance reflects real similarity

> This is why preprocessing matters.

---

## Distance Shapes Model Behavior

**Distance affects:**
- Nearest neighbors
- Clustering boundaries
- Decision surfaces
- Gradient updates

> Changing how distance is measured  
> can completely change model results.

> **This is not a detail.  
> It's a design choice.**

---

## The Big Takeaway

**You should remember this:**

| **Concept** | **Purpose** |
|:------------|:------------|
| **Vectors** | Represent things |
| **Norms** | Measure size |
| **Distance** | Measures similarity |
| **Similarity** | Drives decisions |

> **Machine learning is geometry  
> before it is algorithms.**

---

---

## What's Next

> **Next video:**  
> ### *Dot Product and Projection*

We'll see how alignment,  
not just distance,  
powers predictions and attention.
