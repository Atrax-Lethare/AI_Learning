# Summations: Notation

To read AI research, you must be fluent in Sigma ($\sum$) and Pi ($\prod$) notation.

## 1. Sigma Notation ($\sum$)

The symbol $\sum$ is the Greek letter Sigma, and it stands for **Summation**.

$$\sum_{i=m}^{n} a_i$$

**Breaking it down:**
- **$i$**: The **index of summation**. This is the variable that changes.
- **$m$**: The **lower bound**. This is where the loop starts.
- **$n$**: The **upper bound**. This is where the loop ends.
- **$a_i$**: The **term**. This is the rule for what is being added.

**Example**:
$$\sum_{i=1}^{4} i^2 = 1^2 + 2^2 + 3^2 + 4^2 = 1 + 4 + 9 + 16 = 30$$

## 2. Product Notation ($\prod$)

Sometimes we don't want to add; we want to multiply. For this, we use the Greek letter Pi ($\prod$).

$$\prod_{i=m}^{n} a_i$$

**Example**:
$$\prod_{i=1}^{3} (i+1) = (1+1) \times (2+1) \times (3+1) = 2 \times 3 \times 4 = 24$$

**AI Connection**: The product notation is used heavily in **Probability**. To find the joint probability of independent events, you multiply their individual probabilities: $P(X) = \prod P(x_i)$.

## 3. Common Patterns and Properties

### Linearity
You can pull a constant out of a sum:
$$\sum (c \cdot a_i) = c \cdot \sum a_i$$

### Splitting Sums
The sum of a sum is the sum of the individual sums:
$$\sum (a_i + b_i) = \sum a_i + \sum b_i$$

These properties are essential for simplifying the derivatives of loss functions.
