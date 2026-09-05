# Algebra: Challenges

## Level 1: Conceptual Understanding

**1. The Scale Trap**
You are building a model to predict health risks.
Feature A: Heart Rate (60-100 bpm)
Feature B: Blood Pressure (80-180 mmHg)
Feature C: White Blood Cell Count (4,000-11,000 cells/µL)

If you do NOT normalize these features, which one will likely dominate the model's early training? Why?

**2. The Balance Scale**
In your own words, explain why "doing the same thing to both sides of an equation" is the fundamental rule of algebra. What happens if you forget to do it to one side?

## Level 2: Mathematical Reasoning

**3. Solving for the Weight**
Your model has a simple linear rule: $\text{Output} = w \cdot \text{Input} + b$.
You know:
- $\text{Input} = 10$
- $\text{Output} = 50$
- $b = 5$

Solve for $w$.

**4. Normalization Calculation**
You have a dataset of ages: $[20, 30, 40, 50, 60]$.
- Calculate the Min-Max normalized value for the age `30`.
- Calculate the Mean ($\mu$) and Standard Deviation ($\sigma$).
- Calculate the Z-score for the age `30`.

## Level 3: AI Architecture Reasoning

**5. The Vanishing Bias**
What would happen to a neural network if you set all bias terms $b$ to exactly $0$? Would the model still be able to learn? What specific types of relationships would it be unable to represent?

**6. Regularization Trade-off**
In the equation $\text{Total Loss} = \text{Error} + \lambda \sum w^2$, you notice that as you increase $\lambda$, the weights $w$ get smaller and smaller, eventually all becoming near $0$.
- What does this do to the model's ability to fit the training data?
- Is this a good thing or a bad thing? When would you want this to happen?
