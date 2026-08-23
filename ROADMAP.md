# Process:

**Theory → intuitive understanding → doubts → “go on” → challenge → your solution → evaluation → “go on” → next concept**

# AI Research + AI Engineering Curriculum

## Overall architecture

```text
                         AI MASTERY
                             │
              ┌──────────────┴──────────────┐
              │                             │
       MATHEMATICS TRACK              AI CONCEPTS TRACK
              │                             │
       Linear Algebra                  AI Foundations
       Calculus                        ML Foundations
       Probability                     Classical ML
       Statistics                      Neural Networks
       Optimization                    Deep Learning
              │                        Representation Learning
              │                        Generative AI
              │                        Transformers
              │                        LLMs
              │                        Multimodal AI
              │                        RL
              │                        Modern AI Research
              │                             │
              └──────────────┬──────────────┘
                             │
                       AI ENGINEERING
                             │
              ┌──────────────┼──────────────┐
              │              │              │
          Data/ETL        Training       Deployment
              │              │              │
              └──────────────┼──────────────┘
                             │
                       AI APPLICATIONS
                             │
                  ┌──────────┼──────────┐
                  │          │          │
                 RAG       Agents     AI APIs
                  │          │          │
                  └──────────┼──────────┘
                             │
                      PRODUCTION AI
                             │
               Evaluation • Monitoring
               Optimization • Scaling
               Safety • MLOps
                             │
                       AI RESEARCH
```

There will be **two tracks initially**.

The Mathematics track gives the mathematical intuition and tools required by the AI concepts. Once the minimum mathematical foundation has been reached, **the structured Math track is dropped** from this curriculum. Mathematics is separately coontinued using the other curriculum.

---

# TRACK 1: MATHEMATICS

The objective is **not** “learn mathematics.”

The objective is:

> **Understand enough mathematics to understand what AI models are actually doing.**

You don't need to become a mathematician before touching ML.

## M1. Mathematical Foundations

### M1.1 Functions

* What a function actually represents
* Inputs → transformations → outputs
* Domain and range
* Composition
* Inverse functions
* Why functions are fundamental to ML

### M1.2 Exponents and logarithms

* Exponential growth
* Logarithms as inverse growth
* Why `e` appears everywhere
* Log probabilities
* Log loss
* Numerical stability

### M1.3 Basic algebra

* Equations
* Inequalities
* Rearranging expressions
* Summation notation
* Products
* Ratios
* Normalization

---

# M2. Linear Algebra

This is the **first major mathematical foundation for AI**.

### M2.1 Scalars

### M2.2 Vectors

* What a vector really represents
* Vector as a point
* Vector as direction
* Vector as a collection of features

### M2.3 Vector operations

* Addition
* Subtraction
* Scalar multiplication

### M2.4 Dot product

* Geometric intuition
* Similarity
* Projection
* Why neural networks love dot products

### M2.5 Norms and distance

* L1
* L2
* Euclidean distance
* Cosine similarity

### M2.6 Matrices

* Matrix as a transformation
* Matrix as structured data
* Matrix multiplication
* Why dimensions matter

### M2.7 Matrix transformations

* Scaling
* Rotation
* Projection
* Linear transformations

### M2.8 Systems of equations

### M2.9 Eigenvalues and eigenvectors

* Intuition first
* Why some directions remain special under transformations

### M2.10 High-dimensional spaces

* Dimensionality
* Geometry in AI
* Embeddings
* Curse of dimensionality

---

# M3. Calculus

You don't initially need the full mathematical universe of calculus.

You need to understand **change**.

### M3.1 Limits

### M3.2 Derivatives

* Derivative as rate of change
* Slope
* Sensitivity

### M3.3 Partial derivatives

* Multiple inputs
* How one variable affects the output

### M3.4 Gradients

* Gradient as a direction
* Gradient as a map of local improvement

### M3.5 Chain rule

* The single most important calculus idea for neural networks
* Why nested functions can still be differentiated

### M3.6 Optimization intuition

* Minima
* Maxima
* Local vs global minima
* Landscape intuition

---

# M4. Probability

This becomes extremely important once you start dealing with uncertainty.

### M4.1 Probability fundamentals

### M4.2 Random variables

### M4.3 Probability distributions

### M4.4 Conditional probability

### M4.5 Independence

### M4.6 Bayes' theorem

### M4.7 Expected value

### M4.8 Variance and standard deviation

### M4.9 Common distributions

* Bernoulli
* Binomial
* Gaussian
* Uniform
* Categorical

### M4.10 Joint probability

### M4.11 Marginal probability

### M4.12 Likelihood

### M4.13 Maximum likelihood intuition

---

# M5. Statistics

### M5.1 Population vs sample

### M5.2 Mean, median and mode

### M5.3 Variance and covariance

### M5.4 Correlation

### M5.5 Sampling

### M5.6 Estimation

### M5.7 Bias and variance

### M5.8 Confidence intervals

### M5.9 Hypothesis testing

### M5.10 Statistical significance

### M5.11 Experimental design

### M5.12 Data distributions

This becomes particularly important for **evaluating AI systems rather than merely building them**.

---

# M6. Optimization

This is the bridge between mathematics and machine learning.

### M6.1 Objective functions

### M6.2 Loss functions

### M6.3 Gradient descent

### M6.4 Learning rate

### M6.5 Batch vs stochastic optimization

### M6.6 Momentum

### M6.7 Adaptive optimizers

* AdaGrad
* RMSProp
* Adam

### M6.8 Convex vs non-convex optimization

### M6.9 Regularization

### M6.10 Optimization landscapes

---

# Mathematics Exit Point

Once you have reached approximately:

**Functions → vectors → matrices → derivatives → gradients → probability → statistics → optimization**

we will **pause the structured Mathematics track**.

You continue deeper mathematics separately.

From that point onward, whenever an AI concept requires additional mathematics, I'll tell you:

> **Mathematical prerequisite: X**

and we can connect it back to your mathematics curriculum.

---

# TRACK 2: AI CONCEPTS

Now the fun begins.

And by “fun,” I mean the point where a seemingly innocent equation eventually turns into a model consuming 80 GB of VRAM.

---

# A1. What Is Artificial Intelligence?

Before machine learning, you need a proper conceptual foundation.

### A1.1 Intelligence

* What does “intelligence” actually mean?
* Prediction vs reasoning
* Learning vs memorization
* Adaptation
* Generalization

### A1.2 AI vs ML vs Deep Learning

* Artificial Intelligence
* Machine Learning
* Deep Learning
* Generative AI

### A1.3 What does it mean for a machine to learn?

### A1.4 Rules vs learned behavior

### A1.5 The fundamental ML problem

You will develop this mental model:

```text
DATA
  ↓
MODEL
  ↓
PREDICTION
  ↓
ERROR
  ↓
LEARNING
  ↓
BETTER MODEL
```

This becomes the foundation for almost everything afterward.

---

# A2. Machine Learning Foundations

### A2.1 Dataset

### A2.2 Features

### A2.3 Labels

### A2.4 Samples

### A2.5 Training

### A2.6 Validation

### A2.7 Testing

### A2.8 Generalization

### A2.9 Overfitting

### A2.10 Underfitting

### A2.11 Data leakage

### A2.12 Bias vs variance

### A2.13 Model capacity

### A2.14 Training vs inference

---

# A3. Supervised Learning

### A3.1 Regression

### A3.2 Classification

### A3.3 Decision boundaries

### A3.4 Loss functions

### A3.5 Evaluation metrics

* Accuracy
* Precision
* Recall
* F1
* ROC-AUC
* MAE
* MSE
* RMSE
* R²

### A3.6 Baselines

An important research habit:

> **Never celebrate a model before comparing it against a sensible baseline.**

---

# A4. Classical Machine Learning

We will actually **build these models**, not merely memorize their names.

### A4.1 Linear Regression

### A4.2 Logistic Regression

### A4.3 k-Nearest Neighbors

### A4.4 Naive Bayes

### A4.5 Decision Trees

### A4.6 Random Forests

### A4.7 Gradient Boosting

### A4.8 XGBoost-style boosting

### A4.9 Support Vector Machines

### A4.10 Ensemble learning

For each model:

**intuition → mathematics → implementation → training → evaluation → failure modes → engineering use**

---

# A5. Unsupervised Learning

### A5.1 Clustering

### A5.2 k-Means

### A5.3 Hierarchical clustering

### A5.4 DBSCAN

### A5.5 Dimensionality reduction

### A5.6 PCA

### A5.7 Representation learning

### A5.8 Anomaly detection

---

# A6. Data Engineering for AI

This is where AI engineering starts becoming distinct from simply knowing ML.

### A6.1 Data collection

### A6.2 Data cleaning

### A6.3 Data transformation

### A6.4 Feature engineering

### A6.5 Data pipelines

### A6.6 Train/validation/test pipelines

### A6.7 Dataset versioning

### A6.8 Data quality

### A6.9 Data augmentation

### A6.10 Synthetic data

### A6.11 Data-centric AI

You'll learn an uncomfortable truth here:

> A mediocre model with excellent data can beat an excellent model trained on garbage.

---

# A7. Neural Networks

This is the major transition into deep learning.

### A7.1 Artificial neuron

### A7.2 Weights

### A7.3 Bias

### A7.4 Linear transformation

### A7.5 Activation functions

* Sigmoid
* Tanh
* ReLU
* Leaky ReLU
* GELU
* Softmax

### A7.6 Forward propagation

### A7.7 Loss

### A7.8 Backpropagation

### A7.9 Gradient descent

### A7.10 Computational graphs

### A7.11 Parameter initialization

### A7.12 Learning dynamics

---

# A8. Deep Learning

### A8.1 Deep vs shallow networks

### A8.2 Vanishing gradients

### A8.3 Exploding gradients

### A8.4 Normalization

### A8.5 Batch normalization

### A8.6 Layer normalization

### A8.7 Dropout

### A8.8 Weight decay

### A8.9 Learning-rate schedules

### A8.10 Early stopping

### A8.11 Hyperparameter tuning

### A8.12 Experiment tracking

---

# A9. Computer Vision

### A9.1 Images as tensors

### A9.2 Convolution

### A9.3 Kernels

### A9.4 CNNs

### A9.5 Pooling

### A9.6 Feature maps

### A9.7 ResNet

### A9.8 Object detection

### A9.9 Segmentation

### A9.10 Vision Transformers

### A9.11 Multimodal vision

---

# A10. Sequence Models

### A10.1 Sequential data

### A10.2 Recurrent Neural Networks

### A10.3 Hidden states

### A10.4 LSTM

### A10.5 GRU

### A10.6 Encoder-decoder architectures

### A10.7 Attention

This section is important because it leads directly into Transformers.

---

# A11. Transformers

This will be a **deep section**, because Transformers are foundational to modern AI.

### A11.1 Why recurrence wasn't enough

### A11.2 Attention intuition

### A11.3 Query, Key, Value

### A11.4 Self-attention

### A11.5 Scaled dot-product attention

### A11.6 Multi-head attention

### A11.7 Positional information

### A11.8 Transformer blocks

### A11.9 Residual connections

### A11.10 Layer normalization

### A11.11 Encoder

### A11.12 Decoder

### A11.13 Encoder-decoder Transformers

### A11.14 Computational complexity

### A11.15 Context windows

---

# A12. Large Language Models

### A12.1 Tokenization

### A12.2 Embeddings

### A12.3 Language modeling

### A12.4 Next-token prediction

### A12.5 Pretraining

### A12.6 Scaling

### A12.7 Instruction tuning

### A12.8 Supervised fine-tuning

### A12.9 Preference optimization

### A12.10 RLHF

### A12.11 DPO-style methods

### A12.12 Inference

### A12.13 Temperature

### A12.14 Sampling

### A12.15 Hallucination

### A12.16 Context limitations

### A12.17 Emergent capabilities

### A12.18 Reasoning models

---

# A13. Generative AI

### A13.1 What generation actually means

### A13.2 Autoregressive models

### A13.3 Autoencoders

### A13.4 Variational Autoencoders

### A13.5 GANs

### A13.6 Diffusion models

### A13.7 Text generation

### A13.8 Image generation

### A13.9 Audio generation

### A13.10 Video generation

---

# A14. Embeddings and Representation Learning

### A14.1 What an embedding actually represents

### A14.2 Semantic spaces

### A14.3 Similarity

### A14.4 Dense representations

### A14.5 Sentence embeddings

### A14.6 Image embeddings

### A14.7 Multimodal embeddings

### A14.8 Embedding search

### A14.9 Vector databases

---

# A15. Retrieval-Augmented Generation

### A15.1 Why LLMs need external knowledge

### A15.2 Retrieval

### A15.3 Chunking

### A15.4 Embeddings

### A15.5 Vector search

### A15.6 Hybrid search

### A15.7 Reranking

### A15.8 Context construction

### A15.9 Generation

### A15.10 RAG evaluation

### A15.11 Advanced RAG

* Query rewriting
* Multi-query retrieval
* HyDE
* Parent-child retrieval
* Graph RAG
* Agentic retrieval

---

# A16. AI Agents

### A16.1 What makes an AI system an agent?

### A16.2 Tools

### A16.3 Planning

### A16.4 Memory

### A16.5 Tool calling

### A16.6 ReAct-style systems

### A16.7 Agent loops

### A16.8 Multi-agent systems

### A16.9 Agent evaluation

### A16.10 Reliability problems

---

# A17. Reinforcement Learning

### A17.1 Agent

### A17.2 Environment

### A17.3 State

### A17.4 Action

### A17.5 Reward

### A17.6 Policy

### A17.7 Value

### A17.8 Q-learning

### A17.9 Deep Q Networks

### A17.10 Policy gradients

### A17.11 Actor-critic

### A17.12 PPO

### A17.13 Exploration vs exploitation

### A17.14 RL from human feedback

---

# A18. AI Engineering

Now we move from **building models** to building **systems around models**.

### A18.1 Model APIs

### A18.2 Model serving

### A18.3 REST APIs

### A18.4 FastAPI

### A18.5 Batch inference

### A18.6 Real-time inference

### A18.7 GPU inference

### A18.8 Model serialization

### A18.9 Docker

### A18.10 Cloud deployment

### A18.11 GPU infrastructure

### A18.12 Queues

### A18.13 Caching

### A18.14 Databases

### A18.15 Vector databases

### A18.16 Authentication

### A18.17 Rate limiting

### A18.18 Observability

---

# A19. MLOps

### A19.1 Experiment tracking

### A19.2 Model versioning

### A19.3 Dataset versioning

### A19.4 Model registry

### A19.5 CI/CD for ML

### A19.6 Training pipelines

### A19.7 Deployment pipelines

### A19.8 Monitoring

### A19.9 Data drift

### A19.10 Concept drift

### A19.11 Model degradation

### A19.12 Retraining

---

# A20. AI Evaluation

This gets special emphasis because **building something that works once is not AI engineering**.

### A20.1 Evaluation datasets

### A20.2 Offline evaluation

### A20.3 Online evaluation

### A20.4 Benchmarking

### A20.5 Error analysis

### A20.6 Model comparison

### A20.7 LLM evaluation

### A20.8 RAG evaluation

### A20.9 Agent evaluation

### A20.10 Human evaluation

### A20.11 Automated evaluation

### A20.12 Statistical reliability

---

# A21. AI Optimization

### A21.1 Quantization

### A21.2 Pruning

### A21.3 Knowledge distillation

### A21.4 LoRA

### A21.5 QLoRA

### A21.6 Efficient inference

### A21.7 KV caching

### A21.8 Batching

### A21.9 Speculative decoding

### A21.10 Model compression

### A21.11 GPU optimization

---

# A22. AI Safety and Reliability

### A22.1 Hallucination

### A22.2 Robustness

### A22.3 Adversarial examples

### A22.4 Prompt injection

### A22.5 Data poisoning

### A22.6 Jailbreaking

### A22.7 Model uncertainty

### A22.8 Interpretability

### A22.9 Alignment

### A22.10 AI security

---

# A23. AI Research

This is where the curriculum stops being primarily about **using existing knowledge** and starts teaching you how to **produce new knowledge**.

### A23.1 Reading papers

### A23.2 Understanding papers

### A23.3 Reproducing results

### A23.4 Designing experiments

### A23.5 Ablation studies

### A23.6 Establishing baselines

### A23.7 Hypothesis formation

### A23.8 Experimental controls

### A23.9 Statistical analysis

### A23.10 Benchmark design

### A23.11 Research engineering

### A23.12 Writing research reports

### A23.13 Identifying research gaps

### A23.14 Developing novel architectures

### A23.15 Reproducible research

---

# A24. Capstone Projects

We won't finish with a certificate-shaped piece of paper and a motivational quote. You'll build things.

### Project 1: Classical ML System

**Dataset → preprocessing → model → evaluation → API**

### Project 2: Neural Network

Build and train a neural network **from scratch with NumPy**, then reproduce it using PyTorch.

### Project 3: Computer Vision System

Train and deploy an image classifier.

### Project 4: Transformer

Implement a simplified Transformer yourself.

### Project 5: LLM Fine-Tuning

Fine-tune an open-source model using an efficient technique such as LoRA.

### Project 6: Production RAG

Build:

```text
Documents
   ↓
Ingestion
   ↓
Chunking
   ↓
Embeddings
   ↓
Vector DB
   ↓
Retrieval
   ↓
Reranking
   ↓
LLM
   ↓
Answer
   ↓
Evaluation
```

### Project 7: AI Agent

Build an agent capable of:

```text
Understand task
      ↓
Plan
      ↓
Choose tool
      ↓
Execute
      ↓
Observe result
      ↓
Re-plan
      ↓
Final answer
```

### Project 8: Production AI System

A complete system with:

**data → training → evaluation → model registry → API → deployment → monitoring → retraining**

### Project 9: Research Project

You will:

1. Select a research problem.
2. Read relevant literature.
3. Establish baselines.
4. Form a hypothesis.
5. Implement an experiment.
6. Run ablations.
7. Analyze results.
8. Draw conclusions.
9. Produce a research-style report.

---

# How We Will Actually Study Each Concept

This is important.

I **will not** dump the entire theory of linear regression on you and then hand you a 40-question worksheet like an educational vending machine.

Every concept follows this exact loop:

### Phase 1: Concept

I'll explain:

* **What it is intuitively**
* **Why it exists**
* **What problem it solves**
* **What is happening internally**
* **How the mathematics describes it**
* **How it appears in real AI systems**
* **Common misconceptions**
* **Python implementation where appropriate**

### Phase 2: Your doubts

You ask whatever you don't understand.

I'll keep drilling into the concept until the mental model is solid.

### Phase 3: Challenge

When you say **“go on”**, I give you a challenge.

Not:

> “Define gradient descent.”

That's trivia.

Instead:

> Here's a situation. Predict what the model will do, explain why, and possibly implement it.

The goal is **reasoning**, not memorization.

### Phase 4: Evaluation

You submit your answer/code.

I'll evaluate:

* Conceptual correctness
* Reasoning
* Technical correctness
* Code quality
* Engineering thinking
* Research thinking
* What you missed
* What could be improved

### Phase 5: Next concept

When you say **“go on”**, we advance.

---

# The Most Important Learning Principle

Throughout this curriculum, I'll continually distinguish between four levels:

### Level 1: Know

> “I know what gradient descent is.”

### Level 2: Understand

> “I understand why gradient descent works.”

### Level 3: Build

> “I can implement gradient descent.”

### Level 4: Reason

> “Given a strange training failure, I can determine whether the problem is the optimizer, learning rate, data, architecture, loss, or something else.”

**Our target is Level 4.**

That is the difference between someone who has completed an ML course and someone who can actually engineer or research ML systems.

---

# Starting Point

Before jumping into neural networks and sprinkling the word *Transformer* over everything, we start here:

## Mathematics Track

**M1 → Functions, algebra, exponents/logarithms**

then

**M2 → Linear algebra**

then

**M3 → Calculus**

then

**M4 → Probability**

then

**M5 → Statistics**

then

**M6 → Optimization**

The mathematical minimum needed to begin AI will be established along the way.

## AI Track

**A1 → What is AI and what does it mean for a machine to learn?**

Then:

```text
AI Foundations
      ↓
Machine Learning
      ↓
Classical ML
      ↓
Neural Networks
      ↓
Deep Learning
      ↓
Transformers / LLMs
      ↓
Generative AI
      ↓
RAG / Agents
      ↓
AI Engineering
      ↓
MLOps
      ↓
Evaluation
      ↓
Optimization
      ↓
Safety
      ↓
Research
```

### One deliberate choice

We will **not start with Python ML libraries**.

You already know Python and are strengthening intermediate/advanced Python. The first goal is to understand **what the algorithms are doing**. When appropriate, we'll implement things ourselves with basic Python/NumPy before using PyTorch or higher-level frameworks.

Otherwise you get the classic modern-AI tragedy:

```python
model.fit(X, y)
```

and the human confidently announces that they have trained an AI model while having absolutely no idea what happened between `(` and `)`.

---

## First milestone

Your first major milestone will be:

> **Understand the mathematical and conceptual machinery behind a model well enough that you can implement a simple learning algorithm yourself, explain why it learns, diagnose when it fails, and then use a framework to build it efficiently.**

After that, the difficulty rises substantially.

**Curriculum proposed.** Once you approve it, we begin with **Mathematics M1: Functions**, while keeping the AI track ready in parallel.
