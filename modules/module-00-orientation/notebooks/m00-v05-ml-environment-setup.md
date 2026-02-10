# Setting Up a Professional ML Environment

---

## Why Environment Setup Matters

Many people struggle with machine learning not because of math or models,
but because of:

- **broken environments**
- **dependency conflicts**
- **random installation errors**
- **unclear tooling choices**

> A bad environment creates friction.  
> A good environment lets you focus on learning.

---

## The Principle We Follow

> **Boring tools beat fancy tools.**

**This course prioritizes:**
- **stability**
- **reproducibility**
- **simplicity**

> If your tools are unstable, your learning will be unstable.

---

## What You Need (Minimal)

| **Do NOT Need** | **DO Need** |
|:----------------|:------------|
| Expensive hardware | **Python** |
| Cloud GPUs | **Isolated environment** |
| Complex IDEs | **Code editor** |
| Fancy frameworks | **Version control** |

---

## Step 1 — Python Version

**Use:** **Python 3.10 or newer**

**Check your version:**
```bash
python --version
```

> If this command fails, Python is not installed correctly.

---

## Step 2 — Environment Isolation

> **Never install ML libraries globally.**

**Choose ONE:**
- `venv`
- `conda`

**Example using `venv`:**

```bash
python -m venv .venv
```

**Activate it:**

| **Platform** | **Command** |
|:-------------|:------------|
| **Windows** | `.venv\Scripts\activate` |
| **macOS / Linux** | `source .venv/bin/activate` |

> You should now see the environment name in your terminal.

---

## Step 3 — Core Libraries

**Install the basics:**

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

**For deep learning:**

```bash
pip install torch torchvision
```

> We intentionally keep the stack small.

---

## Step 4 — Sanity Check

**Open Python and run:**

```python
import numpy as np
import torch

x = torch.tensor([1.0, 2.0, 3.0])
print(x * 2)
```

> If this works, your environment is healthy.

---

## Step 5 — Jupyter Notebook

**Start Jupyter:**

```bash
jupyter notebook
```

**Check that:**
- A notebook opens in the browser
- Cells run without errors
- Imports work correctly

> Jupyter will be used throughout this course.

---

## Step 6 — Code Editor

**Recommended:**
- **VS Code**
- **Cursor**

**Why:**
- Python support
- Notebook support
- Git integration
- Lightweight and stable

> Avoid switching editors constantly.

---

## Step 7 — Version Control (Git)

> **Machine learning without version control is risky.**

**Initialize a repository:**

```bash
git init
git status
```

| **Track** | **Do NOT Track** |
|:----------|:-----------------|
| Code | Large datasets |
| Configs | Generated outputs |
| Notebooks | Environment folders |
| Experiment logic | |

---

## What You Should Have Now

**At this point:**
- Python runs correctly
- ML libraries import successfully
- Jupyter works
- Your environment is isolated

> That's all you need to continue.

---

## What We Avoid (For Now)

**At this stage, we intentionally avoid:**
- Docker
- Cloud platforms
- MLOps frameworks
- Over-engineering

> Those tools matter later — not now.

---

## Why This Setup Works Long-Term

**This setup:**
- Scales with your skills
- Works for math, ML, DL, and AI engineering
- Mirrors real professional workflows
- Minimizes distractions

> You can now focus on understanding, not debugging.

---

---

## What's Next

> **Next module:**  
> ### *Mathematics for Machine Learning*

We'll build intuition first  
and connect math directly to models.

> This is where real understanding begins.