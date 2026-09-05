# Exponents and Logarithms: Formalization

To use exponents and logarithms in AI, we need to be comfortable with their algebraic properties. These rules allow us to simplify complex loss functions into something we can actually differentiate.

## 1. The Rules of Exponents

Given a base $a$ and exponents $m, n$:

| Rule | Formula | Intuition |
| :--- | :--- | :--- |
| **Product** | $a^m \cdot a^n = a^{m+n}$ | Adding exponents is like combining growth periods. |
| **Quotient** | $\frac{a^m}{a^n} = a^{m-n}$ | Subtracting exponents is like reversing growth. |
| **Power of Power** | $(a^m)^n = a^{m \cdot n}$ | Scaling the growth rate. |
| **Negative Exp** | $a^{-n} = \frac{1}{a^n}$ | Negative growth is just shrinking (decay). |
| **Zero Power** | $a^0 = 1$ | The starting point before any growth occurs. |

## 2. The Rules of Logarithms

The logarithm is the inverse: if $b^y = x$, then $\log_b(x) = y$.

| Rule | Formula | Why it's useful in AI |
| :--- | :--- | :--- |
| **Product** | $\log_b(M \cdot N) = \log_b(M) + \log_b(N)$ | Turns product of probabilities into a sum of log-probs. |
| **Quotient** | $\log_b(\frac{M}{N}) = \log_b(M) - \log_b(N)$ | Simplifies ratios (like in Likelihood Ratios). |
| **Power** | $\log_b(M^k) = k \cdot \log_b(M)$ | Pulls the exponent down, making it a simple multiplier. |
| **Change of Base** | $\log_b(x) = \frac{\log_a(x)}{\log_a(b)}$ | Allows converting any log to natural log ($\ln$). |

## 3. The Natural Base $e$ and $\ln$

In AI, we almost exclusively use the natural logarithm $\ln(x)$, which is $\log_e(x)$.

**The most important identity in AI mathematics:**
$$\frac{d}{dx} e^x = e^x$$
The derivative of $e^x$ is itself. This unique property makes $e$ the perfect base for optimization and gradient-based learning.

## 4. Common Values to Recognize

When reading AI papers, these patterns appear constantly:
- $e^0 = 1$
- $\ln(1) = 0$
- $\ln(e) = 1$
- $e^{\ln(x)} = x$
- $\ln(e^x) = x$

These "shortcuts" are essential for simplifying the math behind backpropagation.
