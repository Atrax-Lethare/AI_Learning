# Functions: Challenges

These challenges are designed to test your **reasoning**, not your ability to calculate. Try to answer them before looking for a solution.

## Level 1: Conceptual Understanding

**1. The Determinism Test**
You have a function $f$ that predicts whether an email is spam. You input the same email twice. The first time it says "Spam" (90% confidence). The second time it says "Not Spam" (60% confidence).
- Is this a mathematical function? Why or why not?
- In the context of AI, what might cause this behavior?

**2. The Mapping Question**
If a function's domain is "all images of size $28 \times 28$" and its range is $\{0, 1, \dots, 9\}$, what is this function likely doing?

## Level 2: Mathematical Reasoning

**3. The Layering Puzzle**
Consider three functions:
- $f(x) = x + 2$
- $g(x) = 3x$
- $h(x) = x^2$

What is the result of $h(g(f(x)))$? How does this result differ from $f(g(h(x)))$?

**4. The Inverse Paradox**
Why is it impossible to create a perfect inverse function for $f(x) = x^2$ if the domain is all real numbers? What would you have to change about the domain to make an inverse possible?

## Level 3: AI Architecture Reasoning

**5. The Linear Collapse**
Imagine you build a neural network with 100 layers. Every single layer is a linear transformation ($f(x) = wx + b$).
- Can this network represent a complex, curving decision boundary (e.g., a circle)?
- Why or why not?
- What is the simplest change you could make to the architecture to allow it to represent a circle?

**6. The Domain Crash**
You are deploying a model that expects a domain of normalized values between $[0, 1]$. A user provides an input of $10.5$.
- Mathematically, what happened here?
- Practically, what is the likely result of passing this value through the model's functions?
