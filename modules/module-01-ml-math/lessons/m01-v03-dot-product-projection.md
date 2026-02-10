# Dot Product and Projection
## Measuring Alignment in Machine Learning

---

## Why the Dot Product Matters

If you understand the dot product,  
many ML ideas suddenly make sense:

- **Predictions** in linear models
- **Similarity scoring**
- **Attention mechanisms**
- **Classification decisions**

> The dot product is not just math —  
> it's a way to **measure alignment**.

---

## The Right Intuition

> **Forget the formula for now.**

Think of the dot product as answering one question:

> **How aligned are two vectors?**

| **Alignment** | **Dot Product Value** |
|:--------------|:----------------------|
| Strongly aligned | Large value |
| Orthogonal (unrelated) | Near zero |
| Opposite direction | Negative value |

> This single idea powers a lot of ML.

---

## Alignment vs Distance

| **Concept** | **Question** |
|:------------|:--------------|
| **Distance** | "How far apart are these vectors?" |
| **Dot Product** | "Do these vectors point in the same direction?" |

> Both matter, but they capture **different relationships**.

> In many ML problems,  
> direction matters more than distance.

---

## Linear Models Use Dot Products

**In linear regression or classification:**

- Input features → vector
- Model weights → vector
- Prediction = dot product

**Conceptually:**
> The model checks how aligned the input is with what it has learned.

| **Alignment** | **Prediction** |
|:--------------|:---------------|
| High alignment | Strong prediction |
| Low alignment | Weak prediction |

---

## Projection: Extracting What Matters

**Projection answers:**
> **"How much of one vector lies along another?"**

**In ML terms:**
- Focus on relevant directions
- Ignore irrelevant variation

**Projection helps models:**
- Reduce noise
- Emphasize signal
- Make cleaner decisions

---

## Projection as Feature Importance

**You can think of projection as:**
- Asking which features matter most
- Measuring contribution along learned directions

**This intuition connects directly to:**
- Feature weighting
- Embeddings
- Dimensionality reduction

---

## Cosine Similarity Revisited

Cosine similarity is a **normalized dot product**.

**It measures:**
- Alignment only
- Not magnitude

**This is why it's used for:**
- Text similarity
- Embeddings
- Semantic search

> Two vectors can be different in size,  
> but still mean the same thing.

---

## Dot Products in Neural Networks

**Inside neural networks:**
- Neurons compute dot products
- Layers apply transformations
- Attention compares vectors using dot products

> Deep learning scales this idea —  
> but does not replace it.

> The core operation remains the same.

---

## Why This Is Powerful

**Dot products let models:**
- Compare inputs to learned patterns
- Score relevance
- Decide what to focus on

> **This is not a detail.  
> This is the engine.**

---

## The Big Mental Model

**Remember this:**

| **Concept** | **Measures** |
|:------------|:-------------|
| **Distance** | How far apart |
| **Dot Product** | How aligned |
| **Projection** | How much matters |

> **Machine learning uses geometry  
> to make decisions.**

---

---

## What's Next

> **Next video:**  
> ### *Matrix Multiplication as Transformation*

We'll see how dot products scale up  
to entire datasets and models.
