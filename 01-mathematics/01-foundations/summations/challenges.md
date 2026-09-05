# Summations: Challenges

## Level 1: Conceptual Understanding

**1. The Loop Translation**
Convert the following Python code into Sigma ($\sum$) notation:
```python
result = 0
for i in range(1, 11):
    result += (i * 2)
```

**2. Product vs Sum**
In what AI scenario would you use a $\prod$ (Product) instead of a $\sum$ (Sum)? Give a concrete example related to probability.

## Level 2: Mathematical Reasoning

**3. The Simple Sum**
Calculate the value of:
$$\sum_{i=1}^{3} (2i + 1)$$

**4. The Constant Pull**
Simplify this expression using the linearity property of summations:
$$\sum_{i=1}^{n} (5 a_i + 10 b_i)$$

## Level 3: AI Architecture Reasoning

**5. The Dot Product Mystery**
You have a weight vector $w = [0, 1, 0]$ and an input vector $x = [10, 5, 20]$.
- Calculate the weighted sum $\sum w_i x_i$.
- What does the result tell you about the "importance" of the features in $x$?

**6. The Batch Size Paradox**
You are calculating the Total Loss $\sum_{i=1}^{N} L_i$.
- If you double your batch size $N$, what happens to the Total Loss?
- Why is the Mean Loss $\frac{1}{N} \sum L_i$ a more stable metric for monitoring training?
