# Summations: AI Connection

Summations are not just a way to save ink on paper; they represent the core computational patterns of AI.

## 1. The Dot Product (The Core of the Neuron)

Every single neuron in every single neural network performs a **weighted sum**.

If we have inputs $x = [x_1, x_2, \dots, x_n]$ and weights $w = [w_1, w_2, \dots, w_n]$, the output $z$ is:
$$z = \sum_{i=1}^{n} w_i x_i + b$$

This is the **dot product**. It measures how much the input vector $x$ aligns with the weight vector $w$. If the weights for the most important features are large, the sum will be large, and the neuron will "fire."

## 2. Total Loss (The Objective)

When we train a model, we don't just look at one example. We look at a **batch** of $N$ examples.

To find the total error, we sum the individual losses $L$ for every example $i$ in the batch:
$$\text{Total Loss} = \sum_{i=1}^{N} L(\hat{y}_i, y_i)$$

## 3. Mean Squared Error (MSE)

Most AI researchers prefer the **Average Loss** (Mean) over the Total Loss, because the Average Loss doesn't change just because you increased your batch size.

$$\text{MSE} = \frac{1}{N} \sum_{i=1}^{N} (\hat{y}_i - y_i)^2$$

**Breaking down the MSE sum**:
1. $(\hat{y}_i - y_i)$: Calculate the error for one sample.
2. $(\dots)^2$: Square it (to make it positive and penalize large errors more).
3. $\sum_{i=1}^{N}$: Add up all the squared errors.
4. $\frac{1}{N}$: Average them.

## Summary: Summation in the AI Pipeline

$\text{Inputs} \xrightarrow{\sum w_i x_i} \text{Neuron Output} \xrightarrow{\text{Model}} \text{Predictions} \xrightarrow{\frac{1}{N}\sum \text{Loss}} \text{Final Error}$
