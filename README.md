# Gradient Descent Optimization in Spark

This project explores the implementation of **Stochastic Gradient Descent (SGD)** in a distributed environment using **Apache Spark**.

It focuses on how iterative machine learning algorithms can be adapted to big data frameworks beyond the traditional MapReduce limitations.

---

## Motivation

Big data systems are typically optimized for **data extraction and transformation**, but many machine learning algorithms rely on:

- Iterative optimization
- Frequent parameter updates
- High inter-step communication

These characteristics make them difficult to implement efficiently in classical MapReduce models.

---

## Objective

The goal of this project is to:

- Implement **SGD in Spark**
- Demonstrate distributed optimization for machine learning
- Show how Spark handles iterative computation more effectively than MapReduce

---

## Approach

We design a distributed SGD pipeline where:

- Data is partitioned across Spark workers
- Gradients are computed in parallel
- Parameter updates are aggregated centrally

This allows efficient scaling over large datasets.

---

## Algorithm Overview

1. Initialize model parameters
2. Distribute data across Spark RDDs
3. Compute gradients in parallel
4. Aggregate gradients
5. Update parameters
6. Repeat until convergence

---

## Key Insight

Unlike MapReduce:

- Spark supports **in-memory computation**
- Iterative updates are efficient
- Communication overhead is reduced

This makes it well-suited for machine learning optimization tasks such as SGD.

---

## Use Case

This implementation demonstrates a typical ML scenario:

- Large-scale optimization problem
- Iterative gradient updates
- Distributed computation across clusters

---

## Technologies

```
Apache Spark
PySpark
Python
NumPy
```

---

## 🚀 Conclusion

This project highlights how **Spark enables elegant and scalable implementations of SGD**, overcoming the limitations of traditional MapReduce systems in iterative machine learning workflows.
