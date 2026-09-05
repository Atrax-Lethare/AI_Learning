# Functions: Formalization

Now that we have the intuition of a "transformation machine," let's define the rules and language used to describe these machines precisely.

## 1. Notation and Mapping

In mathematics, we describe a function using this notation:

$$f: X \rightarrow Y$$

This is read as: *"The function $f$ maps elements from set $X$ to set $Y$."*

- **$f$**: The name of the function.
- **$X$**: The **Domain**. This is the set of all possible valid inputs.
- **$Y$**: The **Codomain**. This is the set of all possible outputs the function could potentially produce.

When we apply the function to a specific value $x$, we write:
$$y = f(x)$$
Here, $y$ is the **Image** of $x$ under $f$.

### Example: The "Square" Function
Let's say $f$ takes any real number and squares it.
- **Notation**: $f: \mathbb{R} \rightarrow \mathbb{R}$
- **Rule**: $f(x) = x^2$
- **Input**: $x = 3 \rightarrow$ **Output**: $y = 9$

## 2. Domain and Range

While the *Codomain* is the "target" set, the **Range** is the set of values that *actually* come out of the function.

**Example**: For $f(x) = x^2$, the Codomain is all real numbers ($\mathbb{R}$), but the Range is only non-negative real numbers $[0, \infty)$, because a squared number can never be negative.

**AI Connection**: In AI, we carefully define the domain. If your model expects an image of size $224 \times 224$ pixels, then any input outside that "domain" will cause a crash.

## 3. Composition: The Power of Layering

Composition is the act of using the output of one function as the input to another.

If we have two functions:
1. $f(x) = x + 1$
2. $g(x) = x^2$

The composition $g(f(x))$ means: "First apply $f$, then apply $g$ to the result."
$$g(f(x)) = (x + 1)^2$$

**Crucially, order matters.** $f(g(x))$ would be $x^2 + 1$, which is different.

**AI Connection**: This is the secret sauce of Deep Learning. A "Deep" neural network is simply a massive composition of functions:
$$\text{Output} = f_L(f_{L-1}(...f_2(f_1(\text{Input}))...))$$
Each $f$ is a "layer." By composing many simple functions, we can create a function capable of representing incredibly complex relationships (like the relationship between pixels and the concept of a "cat").

## 4. Inverse Functions: Undoing the Map

An inverse function $f^{-1}$ "undoes" the transformation. If $f(x) = y$, then $f^{-1}(y) = x$.

For an inverse to exist, the function must be **bijective** (one-to-one and onto). Every input has exactly one output, and every output comes from exactly one input.

**Example**:
- $f(x) = 2x$
- $f^{-1}(x) = \frac{x}{2}$

**AI Connection**: In Autoencoders (a type of AI), the **Encoder** is a function $f$ that compresses data, and the **Decoder** is an attempt to learn the inverse function $f^{-1}$ to reconstruct the original data.

## Summary Table

| Term | Intuition | Formal Notation | AI Analogy |
| :--- | :--- | :--- | :--- |
| **Domain** | Valid inputs | $X$ | Input Tensor Shape |
| **Range** | Actual outputs | $\{f(x) \mid x \in X\}$ | Possible Prediction Values |
| **Composition** | Layering | $g(f(x))$ | Neural Network Layers |
| **Inverse** | Reversing | $f^{-1}(y) = x$ | Decoding / Reconstruction |
