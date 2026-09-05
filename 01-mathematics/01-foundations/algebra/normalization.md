# Algebra: Normalization and Scaling

In mathematics, the number `10` is just `10`. But in AI, the **meaning** of `10` depends entirely on the scale of the data.

## 1. The Problem: The "Dominant Feature"

Imagine you are training a model to predict health. You have two features:
1. **Age**: ranges from $0$ to $100$.
2. **Annual Income**: ranges from $0$ to $1,000,000$.

If you put these raw numbers into a model, the **Income** feature will completely dominate the **Age** feature. A change of $1$ in income is negligible, but a change of $1$ in age is huge. The model will effectively ignore age because the income numbers are so much larger.

**To fix this, we must normalize the data.**

## 2. Min-Max Scaling (Normalization)

Min-Max scaling squashes all values into a fixed range, usually $[0, 1]$.

**Formula**:
$$x_{norm} = \frac{x - \min(X)}{\max(X) - \min(X)}$$

- If $x$ is the minimum, $x_{norm} = 0$.
- If $x$ is the maximum, $x_{norm} = 1$.
- Everything else falls in between.

**Use Case**: Use this when you know the bounds of your data (e.g., pixel values are always $0-255$).

## 3. Standardization (Z-Score Normalization)

Standardization transforms the data so that it has a **mean of 0** and a **standard deviation of 1**.

**Formula**:
$$z = \frac{x - \mu}{\sigma}$$
Where:
- $\mu$ = the average (mean) of the data.
- $\sigma$ = the standard deviation (the "spread").

**Use Case**: Use this when your data follows a Gaussian (Normal) distribution or when you have outliers. It's the gold standard for most ML algorithms.

## 4. Why is this mandatory for AI?

Most AI models use **Gradient Descent** to learn. Gradient Descent calculates the "slope" of the loss function.

- If one feature is on a scale of $0-1$ and another is $0-1,000,000$, the loss landscape becomes a **long, skinny valley**.
- The gradient will bounce wildly back and forth across the narrow walls of the valley, taking a long time to reach the bottom.
- By normalizing, we make the loss landscape more **spherical**. The gradient can point directly toward the minimum, making training significantly faster and more stable.

## Summary Table

| Method | Formula | Result Range | Best For... |
| :--- | :--- | :--- | :--- |
| **Min-Max** | $\frac{x - \min}{\max - \min}$ | $[0, 1]$ | Bounded data (Pixels) |
| **Z-Score** | $\frac{x - \mu}{\sigma}$ | $\approx [-3, 3]$ | Gaussian data / General ML |
