# What Machine Learning Really Is
*<sub>and what it is not</sub>*

---

## A Common Misunderstanding

Many people think:

- **Machine Learning** = neural networks
- **Machine Learning** = high accuracy
- **Machine Learning** = lots of data
- **Machine Learning** = calling an API

> These ideas are not completely wrong —  
> but they are **dangerously incomplete**.

---

## A Better Definition

**Machine Learning is:**

> ### **Learning a function from data  
> that generalizes to unseen inputs**

> The goal is **not** to fit the training data.  
> The goal is to work **outside** the training data.

---

## The Core Machine Learning Loop

Every machine learning system can be reduced to this loop:

```text
┌─────────────────────────────────────────┐
│     Machine Learning Loop               │
├─────────────────────────────────────────┤
│  1. Feed data into a model              │
│  2. Generate predictions                │
│  3. Measure error using a loss function │
│  4. Update parameters via optimization  │
│  5. Repeat until convergence            │
└─────────────────────────────────────────┘
```

> **Key Insight:** If you understand this loop,  
> you understand **all** machine learning algorithms.

---

## What the Model Actually Learns

### A model does **not** learn:

- **Rules**
- **Logic**
- **Truth**

### A model **does** learn:

- **Parameters** (`weights`)
- An **input → output mapping**
- A **statistical approximation**

> This is why models can be **confidently wrong**.

---

## Training vs Generalization

> **These two are not the same.**

| **Training** | **Generalization** |
|:------------|:-------------------|
| Performance on data the model has **already seen** | Performance on data the model has **never seen** |
| Can be misleading | What actually matters |

> A model that **memorizes** the training set  
> is **useless** in the real world.

---

## Why Accuracy Can Be a Trap

**High accuracy can hide serious problems:**

- **Data leakage**
- **Overfitting**
- **Wrong metrics**
- **Artificial or biased test sets**

> **Warning:** A model with **99% accuracy**  
> can still **completely fail** in production.

---

## Machine Learning Is About Trade-offs

> **There is no perfect model.**

Every decision involves trade-offs:

| **Trade-off** | **Description** |
|:-------------|:----------------|
| **Bias vs Variance** | Simplicity vs Flexibility |
| **Accuracy vs Latency** | Quality vs Speed |
| **Performance vs Cost** | Results vs Resources |
| **Complexity vs Reliability** | Features vs Stability |

> **Engineering** is choosing  
> which trade-offs you accept.

---

## What This Course Focuses On

**This course emphasizes:**

- **Thinking** before tools
- **Understanding** optimization
- **Failure modes** and limitations
- **Systems**, not demos

> **Key Takeaway:** If you understand **what is being optimized**,  
> every algorithm later will make sense.

---

---

## What's Next

> **Next video:**  
> ### *ML vs Data Science vs AI Engineering*

We'll clarify the **roles**  
and where **AI engineering** fits today.
