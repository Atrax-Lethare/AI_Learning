# Exponents and Logarithms: Challenges

## Level 1: Conceptual Understanding

**1. The Compression Question**
You have two numbers: $10$ and $10,000,000$.
- What is the ratio between them?
- What is the difference between their base-10 logarithms?
- Why is the second answer more useful for a computer trying to store these values?

**2. The $e$ Intuition**
If a model's weights are updated using a continuous growth process, why do we see $e$ appearing in the formulas instead of $2$ or $10$?

## Level 2: Mathematical Reasoning

**3. The Log-Prob Conversion**
You are given the log-probabilities of three words:
- $\ln(P(\text{"The"})) = -0.5$
- $\ln(P(\text{"cat"})) = -4.2$
- $\ln(P(\text{"sat"})) = -3.8$

Without using a calculator, which word is the most probable? How do you know?

**4. The Exponent Simplify**
Simplify the following expression:
$$\ln(e^{2x} \cdot e^{3x})$$
What is the final result?

## Level 3: AI Architecture Reasoning

**5. The Underflow Disaster**
You are implementing a custom loss function. You multiply ten probabilities together: $P_{total} = p_1 \cdot p_2 \cdot \dots \cdot p_{10}$.
The computer suddenly returns `0.0` for $P_{total}$, even though none of the $p_i$ are zero.
- What happened technically?
- How would you rewrite this calculation using logarithms to fix it?

**6. Softmax Behavior**
If you multiply all the input logits $x_i$ by a constant $T$ (called "Temperature"), the softmax becomes:
$$\text{Softmax}(x_i, T) = \frac{e^{x_i/T}}{\sum e^{x_j/T}}$$
- What happens to the probabilities if $T$ becomes very large (e.g., $T=100$)?
- What happens if $T$ becomes very small (e.g., $T=0.01$)?
- How does this relate to the "creativity" of an LLM?
