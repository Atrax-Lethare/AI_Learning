# Algebra: Formalization

To manipulate AI models, you need to be fluent in the "grammar" of algebra. Here are the essential tools for rearranging expressions.

## 1. Basic Operations and Inverses

To isolate a variable, you apply the **inverse operation**.

| Operation | Inverse | Example |
| :--- | :--- | :--- |
| Addition ($+$) | Subtraction ($-$) | $x + a = b \rightarrow x = b - a$ |
| Subtraction ($-$) | Addition ($+$) | $x - a = b \rightarrow x = b + a$ |
| Multiplication ($\cdot$) | Division ($\div$) | $ax = b \rightarrow x = \frac{b}{a}$ |
| Division ($\div$) | Multiplication ($\cdot$) | $\frac{x}{a} = b \rightarrow x = ab$ |
| Power ($x^n$) | Root ($\sqrt[n]{x}$) | $x^2 = a \rightarrow x = \pm\sqrt{a}$ |

## 2. Key Algebraic Properties

These rules allow you to rewrite expressions without changing their value.

### The Distributive Property
$$a(b + c) = ab + ac$$
In AI, this is used constantly when expanding loss functions or calculating gradients across a sum of weights.

### Factoring
The opposite of distribution.
$$ab + ac = a(b + c)$$
Factoring is the key to simplifying complex equations to find the root cause of a value.

### Combining Like Terms
You can only add things that are the same "kind."
$3x + 2y + 5x \rightarrow 8x + 2y$
(You cannot combine $x$ and $y$ unless you know their relationship).

## 3. Inequalities and Constraints

Not every relationship is an equality. Sometimes we have **constraints**.

- $x > 5$: $x$ must be greater than 5.
- $x \leq 1$: $x$ must be 1 or less.

**AI Connection**: In "Constrained Optimization," we try to find the best weights $w$ such that some condition is met (e.g., "the total sum of weights must be less than 1"). This is the basis of **Regularization** (which you will see in M6).

## 4. Rearranging Complex Expressions

When solving for a variable buried in a complex expression, follow the **"Reverse PEMDAS"** (or reverse order of operations) logic:
1. Undo Addition/Subtraction.
2. Undo Multiplication/Division.
3. Undo Exponents/Roots.
4. Undo Parentheses.

**Example**: Solve for $x$ in $3(x - 4)^2 = 12$
1. Divide by 3: $(x - 4)^2 = 4$
2. Square root: $x - 4 = \pm 2$
3. Add 4: $x = 4 \pm 2 \rightarrow \{6, 2\}$
