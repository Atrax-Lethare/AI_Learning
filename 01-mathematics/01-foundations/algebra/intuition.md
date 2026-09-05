# Algebra: The Intuition

## The Problem: Solving for the Unknown

Up until now, we've looked at functions as machines where we provide an input and get an output.
`[ Input ]` $\rightarrow$ `[ Function ]` $\rightarrow$ `[ Output ]`

But in the real world—and especially in AI—we often have the opposite problem. We know the **output** we want, and we know the **function**, but we don't know the **input**.

**Example**: You want your AI model to predict a house price of \$500,000. You know the function is $\text{Price} = 200 \times \text{sqft}$.
Now you have to ask: *"What square footage produces this price?"*

This is the essence of algebra: **working backward to find the unknown.**

## The Mental Model: The Balance Scale

The most important intuition in algebra is the **Balance Scale**.

Imagine an equation like $2x + 5 = 15$ as a scale in perfect balance.
- The left side ($2x + 5$) weighs exactly the same as the right side ($15$).

To find $x$, you must strip away everything around it. But to keep the scale balanced, **any operation you perform on one side must be performed on the other.**

1. **Subtract 5 from both sides**: $2x = 10$ (Scale is still balanced).
2. **Divide both sides by 2**: $x = 5$ (Scale is still balanced).

## Algebra as the "Language of Rules"

Algebra isn't just about finding $x$. It's about describing relationships using symbols so that we can manipulate them without knowing the exact numbers yet.

In AI, we don't just solve for one $x$. We solve for millions of $w$ (weights) and $b$ (biases). We use algebra to derive the "Update Rule" that tells the computer exactly how to change those weights to reduce the error.

If you can't rearrange a simple equation, you will find it impossible to understand how a model "learns." Algebra is the tool we use to move the "error" from the output side of the equation back to the input side, where we can fix it.
