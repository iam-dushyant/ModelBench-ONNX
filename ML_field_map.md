# Personal ML Field Map

## Purpose of This Document

This document provides a basic, structured overview of the main areas of machine learning that are relevant to building practical ML engineering capability.

The goal is not to become an expert in every area immediately. The goal is to understand the landscape, how the topics connect, and what skills or portfolio evidence can be built over time.

## Target Direction

My target direction is practical machine learning engineering, with emphasis on:

* understanding core machine learning concepts;
* building and evaluating models;
* understanding modern deep learning and transformer-based systems;
* learning how models are exported, deployed, served, monitored, and maintained;
* developing portfolio evidence that demonstrates practical capability.

---

# 1. Classical Machine Learning

## What It Means

Classical machine learning refers to traditional ML techniques that learn patterns from data without relying on deep neural networks.

These methods are still widely used in real-world systems because they are often:

* easier to understand;
* faster to train;
* cheaper to run;
* effective on structured/tabular data;
* easier to explain to business or engineering teams.

## Common Topics

Examples of classical ML methods include:

* linear regression;
* logistic regression;
* decision trees;
* random forests;
* gradient boosting;
* support vector machines;
* k-means clustering;
* principal component analysis.

## Typical Use Cases

Classical ML is often used for:

* predicting prices or demand;
* classifying customers or transactions;
* detecting fraud;
* ranking leads;
* forecasting business outcomes;
* clustering users into groups;
* identifying patterns in structured data.

## Why It Matters

Classical ML builds the foundation for understanding how models learn from data. It also introduces important concepts such as:

* features;
* labels;
* training data;
* test data;
* overfitting;
* underfitting;
* model evaluation;
* accuracy and error.

Even when working with modern deep learning or LLMs, these ideas remain important.

## My Learning Goal

I should be able to:

* explain common ML algorithms at a high level;
* train simple models using Python;
* evaluate model performance;
* understand when classical ML may be more suitable than deep learning.

---

# 2. Deep Learning

## What It Means

Deep learning is a type of machine learning based on neural networks. Neural networks are models made of layers that transform input data into useful predictions.

Deep learning is especially powerful for complex data such as:

* images;
* audio;
* text;
* video;
* large unstructured datasets.

## Common Topics

Important deep learning topics include:

* neural networks;
* layers;
* weights and biases;
* activation functions;
* loss functions;
* gradient descent;
* backpropagation;
* training loops;
* GPUs;
* PyTorch or TensorFlow.

## Typical Use Cases

Deep learning is commonly used for:

* image recognition;
* speech recognition;
* natural language processing;
* recommendation systems;
* fraud detection;
* object detection;
* generative AI;
* large language models.

## Why It Matters

Deep learning is the foundation of many modern AI systems. Understanding it helps explain how advanced systems such as transformers and LLMs work.

For an ML engineer, deep learning is important because it connects model development with practical engineering problems such as:

* training time;
* inference speed;
* hardware requirements;
* memory usage;
* model deployment.

## My Learning Goal

I should be able to:

* understand what a neural network is;
* train a small neural network using PyTorch;
* explain the role of loss functions and optimisation;
* understand the difference between training and inference;
* recognise when deep learning is useful and when it may be unnecessary.

---

# 3. Transformers and Large Language Models

## What It Means

Transformers are a type of deep learning architecture that is especially effective for working with sequences, such as text.

Large language models, or LLMs, are usually built using transformer architectures. They are trained on large amounts of text and can generate, summarise, classify, translate, and reason over language.

## Common Topics

Important transformer and LLM topics include:

* tokens;
* tokenisation;
* embeddings;
* attention;
* self-attention;
* transformer layers;
* pre-training;
* fine-tuning;
* prompting;
* context windows;
* retrieval-augmented generation;
* hallucination;
* inference cost and latency.

## Typical Use Cases

Transformers and LLMs are used for:

* chatbots;
* document summarisation;
* code generation;
* question answering;
* search enhancement;
* classification;
* translation;
* information extraction;
* customer support automation.

## Why It Matters

Transformers and LLMs are central to modern AI. Even if I do not train large models from scratch, I should understand how to use them responsibly and effectively.

For practical ML engineering, it is important to understand:

* how text is converted into tokens;
* how models use context;
* why LLMs can make mistakes;
* how to evaluate output quality;
* how to control cost and latency;
* how to connect LLMs with external data.

## My Learning Goal

I should be able to:

* explain what a transformer is at a high level;
* understand the role of tokens and embeddings;
* use an existing model from Hugging Face or an API;
* understand the difference between prompting, fine-tuning, and retrieval;
* evaluate basic LLM outputs for quality, accuracy, and usefulness.

---

# 4. Model Evaluation

## What It Means

Model evaluation is the process of measuring how well a model performs.

A model is not useful just because it can make predictions. It must be tested to understand whether its predictions are accurate, reliable, fair, efficient, and suitable for the intended use case.

## Common Topics

Important evaluation concepts include:

* training set;
* validation set;
* test set;
* accuracy;
* precision;
* recall;
* F1 score;
* confusion matrix;
* mean squared error;
* latency;
* cost;
* robustness;
* error analysis.

## Typical Use Cases

Evaluation helps answer questions such as:

* Is the model accurate enough?
* What kinds of mistakes does it make?
* Does it perform well on unseen data?
* Is it too slow for production?
* Is it too expensive to run?
* Does it fail on certain types of input?
* Is it better than a simpler baseline model?

## Why It Matters

Evaluation is one of the most important parts of machine learning. A model that performs well in a notebook may fail in production if it has not been properly evaluated.

For LLMs, evaluation is especially important because outputs may sound confident even when they are incorrect.

## My Learning Goal

I should be able to:

* choose appropriate evaluation metrics;
* compare model performance against a baseline;
* identify common error patterns;
* understand trade-offs between accuracy, latency, and cost;
* document evaluation results clearly.

---

# 5. Model Formats

## What It Means

Model formats are the file types or structures used to save, export, and move machine learning models between tools and environments.

A model may be trained in one framework but deployed in another system. Model formats help make this possible.

## Common Topics

Common model formats include:

* PyTorch model files;
* TensorFlow SavedModel;
* ONNX;
* TorchScript;
* Hugging Face model formats;
* model checkpoints.

## What ONNX Means

ONNX stands for Open Neural Network Exchange. It is a format designed to make models portable across different frameworks and runtimes.

For example, a model trained in PyTorch may be exported to ONNX so it can be run using ONNX Runtime in a production environment.

## Why It Matters

Model formats matter because production systems often care about:

* portability;
* performance;
* compatibility;
* inference speed;
* hardware support;
* deployment flexibility.

A model is not fully useful if it only works inside a training notebook. It needs to be packaged and served reliably.

## My Learning Goal

I should be able to:

* understand why models need to be exported;
* save and load a trained model;
* export a simple model to ONNX;
* understand the role of ONNX Runtime;
* explain the difference between training format and deployment format.

---

# 6. Inference Systems

## What It Means

Inference is the process of using a trained model to make predictions on new data.

An inference system is the engineering setup that allows users, applications, or services to send input to a model and receive output.

## Common Topics

Important inference topics include:

* real-time inference;
* batch inference;
* model serving;
* APIs;
* request and response formats;
* latency;
* throughput;
* batching;
* scaling;
* caching;
* monitoring;
* fallback behaviour.

## Real-Time Inference

Real-time inference means the model responds quickly to individual requests.

Examples:

* chatbot response;
* fraud check during payment;
* image classification from an uploaded photo;
* recommendation shown on a website.

## Batch Inference

Batch inference means the model processes many records at once.

Examples:

* scoring all customers overnight;
* generating weekly predictions;
* processing large document sets;
* classifying historical data.

## Why It Matters

Inference is where ML becomes useful to real users or systems. A model must be reliable, fast, and available.

Production inference introduces engineering concerns such as:

* response time;
* server cost;
* model loading time;
* memory usage;
* traffic spikes;
* logging;
* failure handling.

## My Learning Goal

I should be able to:

* explain the difference between training and inference;
* build a simple API around a model;
* understand real-time vs batch inference;
* measure basic latency;
* understand why deployment requires more than just a trained model.

---

# 7. MLOps

## What It Means

MLOps means Machine Learning Operations. It is the practice of managing the full lifecycle of machine learning systems in a reliable, repeatable, and production-ready way.

It combines ideas from:

* machine learning;
* DevOps;
* software engineering;
* data engineering;
* monitoring and operations.

## Common Topics

Important MLOps topics include:

* data versioning;
* model versioning;
* experiment tracking;
* model registry;
* CI/CD for ML;
* automated testing;
* deployment pipelines;
* monitoring;
* retraining;
* rollback;
* drift detection.

## Why ML Needs Operations

Traditional software usually behaves the same way unless the code changes. ML systems can change in behaviour because the data changes.

For example:

* customer behaviour changes;
* fraud patterns change;
* language usage changes;
* product demand changes;
* input data quality gets worse.

This means ML systems need ongoing monitoring.

## Why It Matters

MLOps is important because many ML projects fail not due to model quality, but because they are difficult to deploy, monitor, reproduce, or maintain.

A production ML system should answer:

* Which data trained this model?
* Which model version is currently deployed?
* How well is the model performing?
* Has the data distribution changed?
* Can we roll back to a previous version?
* Can the deployment be repeated reliably?

## My Learning Goal

I should be able to:

* understand the ML lifecycle;
* explain what a model registry is;
* understand why experiment tracking matters;
* build a simple repeatable training and deployment workflow;
* understand the basics of monitoring and retraining.

---

# 8. ML Systems

## What It Means

ML systems focus on the engineering side of making machine learning models work efficiently in real-world environments.

This area is concerned with performance, reliability, memory usage, latency, deployment architecture, and integration with production systems.

## Common Topics

Important ML systems topics include:

* model serving;
* C++;
* Python;
* ONNX Runtime;
* CMake;
* Docker;
* APIs;
* latency optimisation;
* memory optimisation;
* CPU vs GPU inference;
* batching;
* concurrency;
* observability.

## Why C++ Can Matter

Python is widely used for ML training and experimentation. However, C++ is often used where performance, low latency, or system-level integration matters.

Examples:

* running models in high-performance services;
* integrating inference into existing C++ applications;
* reducing runtime overhead;
* deploying models in constrained environments.

## Why It Matters

ML systems knowledge helps bridge the gap between research models and production applications.

A model may be accurate, but if it is too slow, too expensive, or too unreliable, it may not be useful in production.

## My Learning Goal

I should be able to:

* understand how models are served in production;
* run a model through ONNX Runtime;
* understand basic latency and throughput measurements;
* compare Python-based and lower-level inference approaches;
* build small examples that show model deployment and performance awareness.

---

# 9. Portfolio Evidence

## What It Means

Portfolio evidence is the practical proof that I have learned and applied machine learning concepts.

Instead of only saying I understand ML, I should produce visible examples that demonstrate capability.

## Common Portfolio Items

Useful portfolio evidence can include:

* GitHub repositories;
* notebooks;
* Python scripts;
* model training examples;
* model evaluation reports;
* ONNX export examples;
* inference APIs;
* C++ inference examples;
* README files;
* architecture diagrams;
* benchmark results;
* short technical write-ups.

## Why It Matters

Portfolio evidence is important because ML knowledge can be difficult to prove through statements alone.

A good portfolio shows:

* what problem was solved;
* what tools were used;
* how the model was evaluated;
* how the model was deployed or served;
* what trade-offs were considered;
* what could be improved next.

## Good Portfolio Principles

A strong ML portfolio should be:

* clear;
* practical;
* well documented;
* reproducible;
* focused on engineering quality;
* honest about limitations;
* easy for someone else to understand.

## My Learning Goal

I should be able to create portfolio projects that show:

* basic ML model training;
* model evaluation;
* model export;
* inference serving;
* MLOps awareness;
* ML systems awareness;
* clear technical communication.

---

# 10. How These Areas Connect

The machine learning field can be understood as a pipeline:

1. Data is collected and prepared.
2. A model is trained.
3. The model is evaluated.
4. The model is saved or exported.
5. The model is deployed into an inference system.
6. The system is monitored.
7. The model is improved or retrained when needed.

In simple terms:

* Classical ML and deep learning help build models.
* Transformers and LLMs are modern model architectures used heavily in language tasks.
* Model evaluation checks whether models are good enough.
* Model formats make models portable.
* Inference systems make models usable.
* MLOps keeps models reliable over time.
* ML systems make models efficient and production-ready.
* Portfolio evidence proves that these ideas have been applied in practice.

---

# 11. Personal Skill Map

| Area                  | Current Understanding | Target Understanding | Evidence to Build                                |
| --------------------- | --------------------- | -------------------- | ------------------------------------------------ |
| Classical ML          | Basic                 | Confident            | Train and evaluate simple models                 |
| Deep Learning         | Beginner/basic        | Practical            | Build a small neural network                     |
| Transformers and LLMs | Beginner              | Practical            | Use a transformer model for text task            |
| Model Evaluation      | Basic                 | Confident            | Write evaluation report with metrics             |
| Model Formats         | Beginner              | Practical            | Export model to ONNX                             |
| Inference Systems     | Beginner              | Practical            | Build simple API for model inference             |
| MLOps                 | Beginner              | Practical            | Create repeatable training/deployment workflow   |
| ML Systems            | Beginner              | Practical            | Run model using ONNX Runtime and measure latency |
| Portfolio Evidence    | Early stage           | Strong               | Maintain documented GitHub projects              |

---

# 12. Initial Portfolio Plan

## Project 1: Classical ML Baseline

Build a simple model using a structured dataset.

Evidence:

* notebook;
* train/test split;
* model comparison;
* evaluation metrics;
* short README.

## Project 2: Deep Learning Starter

Build a small neural network using PyTorch.

Evidence:

* training loop;
* loss tracking;
* evaluation results;
* explanation of model design.

## Project 3: Transformer Text Task

Use a pre-trained transformer model for a text classification or summarisation task.

Evidence:

* input examples;
* model outputs;
* evaluation notes;
* limitations.

## Project 4: ONNX Export and Inference

Export a trained model to ONNX and run inference using ONNX Runtime.

Evidence:

* export script;
* inference script;
* before/after comparison;
* basic latency measurement.

## Project 5: Simple MLOps Workflow

Create a repeatable workflow for training, saving, evaluating, and serving a model.

Evidence:

* clear folder structure;
* README;
* requirements file;
* automated script;
* simple testing or validation step.

---

# 13. Week 1 Deliverables

By the end of Week 1, I should have:

* created the GitHub repository;
* created the initial folder structure;
* added an initial README;
* documented the local environment setup;
* created this ML field map;
* identified the first portfolio project to build.

---

# 14. Summary

This ML field map gives me a starting point for understanding the machine learning landscape.

The main areas I need to build knowledge in are:

* classical machine learning;
* deep learning;
* transformers and LLMs;
* model evaluation;
* model formats;
* inference systems;
* MLOps;
* ML systems;
* portfolio evidence.

The long-term goal is to move from theoretical understanding to practical evidence by building small, well-documented projects that show real ML engineering capability.

The learning topics are structured as below for reference:

Machine Learning

│

├── Mathematics

│   ├── Linear Algebra

│   ├── Calculus

│   ├── Probability

│   └── Statistics

│

├── Classical ML

│   ├── Regression

│   ├── Trees

│   ├── Ensembles

│   ├── SVM

│   └── Clustering

│

├── Deep Learning

│   ├── CNN

│   ├── RNN

│   ├── Transformers

│   └── Diffusion

│

├── NLP

├── Computer Vision

├── Reinforcement Learning

├── LLMs

├── MLOps

├── Feature Engineering

├── Experiment Tracking

├── Deployment

├── Monitoring

└── AI Infrastructure
