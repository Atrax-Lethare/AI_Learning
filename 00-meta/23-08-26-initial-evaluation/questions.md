A curriculum assumes a starting line; you don't actually know yours yet, and pretending otherwise is how people end up “learning” matrix multiplication for the fourth time.

We'll use a **diagnostic test**, not a conventional exam. It will test whether you can **reason with concepts**, not whether you've memorized terminology.

# AI + Mathematics Diagnostic Test

### Instructions

* **Do not use Google, ChatGPT, notes, or code execution.**
* You may write pseudocode where requested.
* Don't worry about getting things wrong. Wrong answers are useful here.
* For questions involving reasoning, **explain your thinking**, even when you're unsure.
* You can answer all questions in one message.
* For any question you genuinely don't know, write **“I don't know”** rather than guessing.

The test has **5 sections** and increases in difficulty.

---

# Section 1: Mathematical Foundations

### 1. Functions

Suppose:

[
f(x)=2x+3
]

What are:

**a)** (f(2))
**b)** (f(10))
**c)** What does the function actually *do* to its input?

Don't just give the numerical answers for (c).

---

### 2. Algebraic reasoning

If:

[
3x+7=22
]

find (x).

Then explain **why** your steps preserve the equality.

---

### 3. Exponents

Without calculating the exact numerical value:

[
2^{10}
]

is approximately how many times larger than:

[
2^5
]

Explain how you know.

---

### 4. Logarithms

What does this mean conceptually?

[
\log_2(32)=5
]

Explain it without saying only “the answer is 5.”

---

### 5. Graph intuition

Imagine a graph of:

[
y=x^2
]

What happens to the value of (y) when (x) changes from 2 to 3?

More importantly, **how does the rate at which (y) changes compare around (x=2) versus around (x=10)?**

You don't need calculus terminology if you haven't learned it.

---

# Section 2: Linear Algebra

### 6. Vectors

Consider:

[
A=[2,4,6]
]

What could these three numbers represent in a machine-learning problem?

Give **one realistic example**.

---

### 7. Vector addition

Calculate:

[
[1,2,3]+[4,5,6]
]

Then explain what vector addition means geometrically or intuitively.

---

### 8. Dot product

Calculate:

[
[1,2,3]\cdot[4,5,6]
]

Then answer:

**Why do you think dot products are useful for machine learning?**

You don't need to know the formal answer. I care about your reasoning.

---

### 9. Matrices

Suppose:

[
A=
\begin{bmatrix}
1 & 2\
3 & 4
\end{bmatrix}
]

and

[
x=
\begin{bmatrix}
5\
6
\end{bmatrix}
]

What is (Ax)?

Then tell me what you think **matrix multiplication is doing** conceptually.

---

### 10. Dimensions

You have:

```text
A: 3 × 4
B: 4 × 2
```

Can (AB) be calculated?

If yes, what dimensions will the result have?

What about (BA)?

---

# Section 3: Calculus, Probability and Statistics

You are **not expected** to know all of these. This section is partly intended to locate the boundary of your knowledge.

### 11. Derivative intuition

What do you think a derivative tells us?

Explain in your own words.

---

### 12. Simple derivative

If:

[
f(x)=x^2
]

what do you think (f'(x)) is?

If you don't know, say so.

---

### 13. Gradient

You've probably heard the term **gradient** in machine learning.

What do you currently think a gradient is?

Again, “I don't know” is perfectly acceptable.

---

### 14. Probability

A fair six-sided die is rolled once.

What is the probability of getting an even number?

Explain your reasoning.

---

### 15. Conditional probability

Suppose I tell you:

> A randomly selected student is taller than 180 cm.

Does that information change the probability that the student is male?

Why or why not?

Don't worry about having demographic data. I'm testing your understanding of **conditional probability**, not asking for a statistic.

---

### 16. Mean and variance

Consider the two datasets:

```text
A = [5, 5, 5, 5, 5]

B = [1, 3, 5, 7, 9]
```

Both have the same mean.

Which has greater variance?

Explain intuitively **what variance is measuring**.

---

# Section 4: Computer Science + Python

These questions aren't really testing whether you're a Python beginner or intermediate. They're testing whether your programming foundation is sufficient for ML.

### 17. Complexity

What is the approximate time complexity of this code?

```python
for x in numbers:
    print(x)
```

What about:

```python
for x in numbers:
    for y in numbers:
        print(x, y)
```

Explain why.

---

### 18. Data structures

When would you choose:

* `list`
* `set`
* `dict`

Give one practical situation for each.

---

### 19. Functions

What is the difference between:

```python
def add(a, b):
    return a + b
```

and:

```python
def add(a, b):
    print(a + b)
```

Why does that distinction matter when building larger programs?

---

### 20. OOP

Suppose you're building a machine-learning system.

What do you think a **class** could represent?

Give one example.

---

### 21. Debugging

Consider:

```python
numbers = [1, 2, 3, 4, 5]

for i in range(len(numbers)):
    numbers[i] = numbers[i] * 2

print(numbers)
```

What will it output?

Then explain what the code is doing.

---

### 22. Python reasoning

What is the output?

```python
x = [1, 2, 3]

y = x

y.append(4)

print(x)
```

Most importantly, **why**?

---

# Section 5: AI / Machine Learning Intuition

This is the most important section.

You may know very little here. That's completely fine.

### 23. What is machine learning?

Explain in your own words what you think **machine learning** actually means.

Don't give me a textbook definition.

---

### 24. Rules vs learning

Suppose I want a program that identifies whether an email is spam.

Approach A:

```text
IF email contains "free money"
→ spam
```

Approach B:

Give the computer **100,000 emails labeled spam/not-spam** and let it learn patterns.

What is fundamentally different between these two approaches?

---

### 25. Model intuition

Suppose you're trying to predict house prices.

You give a model:

```text
House size
Number of bedrooms
Location
Age
```

and it predicts:

```text
₹1.2 crore
```

What do you think the **model** actually is?

Don't worry about using precise terminology. Tell me what you imagine is happening internally.

---

### 26. Training

What do you think happens when we say:

> “Train the model on this dataset.”

Explain what you think happens **step by step**.

---

### 27. Error

A model predicts:

```text
Actual price:     ₹1 crore
Predicted price:  ₹1.3 crore
```

What should the model do with this information?

Why is the error useful?

---

### 28. Learning

Suppose the model makes:

```text
Prediction 1 → Error = 30
Prediction 2 → Error = 20
Prediction 3 → Error = 12
Prediction 4 → Error = 5
```

What does this suggest is happening?

What would you want to happen next?

---

### 29. Overfitting

Imagine a student memorizes every question and answer from a practice exam.

Then they encounter completely new questions and perform terribly.

What does this remind you of in machine learning?

Explain the analogy.

---

### 30. Training vs testing

Why shouldn't we evaluate a model only on the exact data it trained on?

---

### 31. Neural networks

What do you currently know about a **neural network**?

Tell me everything you believe you know, even if it's incomplete.

---

### 32. Deep learning

What do you think makes **deep learning** different from traditional machine learning?

---

### 33. LLMs

What do you think an LLM such as GPT fundamentally does?

Try to explain it from the inside rather than saying:

> “It is an AI that understands language.”

---

### 34. Transformers

What do you currently know about **Transformers** and **attention**?

Again, “nothing” is a valid answer.

---

# Section 6: Your Reasoning Ability

This is the section I'm especially interested in.

### 35. The debugging problem

You train two models on the same dataset.

```text
Model A
Training accuracy: 99%
Testing accuracy: 72%

Model B
Training accuracy: 91%
Testing accuracy: 89%
```

Which model would you prefer?

**Why?**

---

### 36. Research thinking

You change one component of an AI system and performance increases from:

```text
82% → 84%
```

Can you immediately conclude that your change caused the improvement?

Explain why or why not.

---

### 37. Engineering thinking

Your AI model performs extremely well in your notebook.

You deploy it.

Real users complain that it is slow.

What kinds of things would you investigate?

Give as many plausible causes as you can.

---

### 38. The big one

Imagine you're given a completely unfamiliar AI paper.

What would you do to understand it?

Describe your **process**, not the answer.

---

# Final Self-Assessment

Answer these honestly.

### 39. Rate yourself from 0–5:

| Area             | Rating |
| ---------------- | -----: |
| Algebra          |     /5 |
| Functions        |     /5 |
| Linear algebra   |     /5 |
| Calculus         |     /5 |
| Probability      |     /5 |
| Statistics       |     /5 |
| Python           |     /5 |
| Machine learning |     /5 |
| Deep learning    |     /5 |
| LLMs             |     /5 |
| AI engineering   |     /5 |

### 40. Tell me three things

**A.** Which section felt easiest?

**B.** Which section felt hardest?

**C.** Which question made you think, **“I have absolutely no idea”**?

---

## How I'll use your answers

I won't simply give you a score out of 40. That would be a spectacularly poor diagnostic.

I'll classify you separately on:

**Mathematical readiness**
→ Foundation / Beginner / Intermediate / Advanced

**Programming readiness**
→ Foundation / Beginner / Intermediate / Advanced

**AI conceptual readiness**
→ Foundation / Beginner / Intermediate / Advanced

**Reasoning ability**
→ Developing / Solid / Strong / Research-ready

Then I'll **modify the curriculum we just created** around your actual gaps.

For example, you might turn out to be:

```text
Mathematics       → Beginner
Python            → Intermediate
AI concepts       → Foundation
Reasoning         → Strong
```

In that case, I won't waste your time relearning Python, but I also won't throw you into Transformers because you can write a `for` loop. Humanity has already generated enough premature Transformer tutorials.

**Answer questions 1–40 in your own words.** Your mistakes will be considerably more informative than a collection of correct guesses.
