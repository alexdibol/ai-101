# AI-101 — Machine Learning and Artificial Intelligence Foundations

Mechanics-first · reproducible · transparent · pedagogically structured  
Built for **students, MBA / Master of Finance cohorts, and professional practitioners** who want to understand how machine learning and artificial intelligence systems work at the level of mechanism, training behavior, architectural structure, and observable failure modes.

---

## What this repository is

This repository is the home of **AI-101**: a book-and-notebook laboratory for studying the foundations of machine learning and artificial intelligence in a way that is operational, visual, reproducible, and intellectually honest.

The purpose of this repository is not to mystify AI.  
The purpose is to make AI **legible**.

That means treating models not as magical output engines, but as structured computational systems with explicit inputs, parameters, architectures, objective functions, optimization procedures, training dynamics, inference behavior, limitations, and failure cases.

This repository is designed to help the reader answer questions such as:

- what exactly is being learned
- how training differs from inference
- why one architecture behaves differently from another
- what assumptions are built into each model family
- how errors, instability, and overfitting appear in practice
- why some architectures are better suited for images, sequences, graphs, or generative tasks

This is a **foundations-first** project. It is meant to build understanding before abstraction, before policy overlays, and before production claims.

It is intentionally explicit about what it does **not** claim:

- it does **not** claim production readiness by default
- it does **not** claim state-of-the-art performance
- it does **not** claim business, investment, or deployment value merely because a notebook runs
- it does **not** treat model outputs as self-explanatory truth
- it does **not** replace disciplined technical understanding with buzzwords

**Core premise:**  
**Mechanism first. Interpretation second. Hype never.**

---

## Repository structure

This repository follows the structure shown in this repo:

- **/book/**  
  The book materials. This is the conceptual spine of the project: motivation, theory, mathematical intuition, architectural explanation, practical limits, and chapter-to-chapter progression.

- **/notebooks/**  
  The executable laboratories. These notebooks operationalize the book chapter by chapter through controlled experiments, visualizations, training runs, and model diagnostics.

- **README.md**  
  The repository overview and orientation guide.

---

## Directory layout in this repository

    ai-101/
    ├── book/
    ├── notebooks/
    └── README.md

---

## The book

The **/book/** directory contains the book-level framework for **AI-101**.

The role of the book is not merely to summarize machine learning models in encyclopedic fashion. Its role is to explain, in a structured and cumulative way:

- why each model family emerged
- what computational problem it addresses
- what internal mechanism defines it
- how it learns
- what its strengths are
- where its weaknesses become visible
- why the next chapter is a natural continuation of the previous one

The book is therefore the conceptual architecture of the repository. It provides continuity, theoretical grounding, and pedagogical sequence.

If a compiled PDF is placed inside **/book/**, that file becomes the cleanest single-entry reading version of the project. The source directory, however, remains important because it contains the organized material from which the book is assembled.

---

## The notebooks

The **/notebooks/** directory contains the practical laboratories that accompany the book.

Each notebook is designed to make the corresponding chapter concrete by allowing the learner to:

- generate or inspect data
- define a model
- train it under explicit hyperparameters
- visualize performance and behavior
- compare outputs across settings
- observe failure modes directly
- develop intuition through repeated experimentation

These notebooks are not ornamental supplements. They are the executable half of the learning system.

The book explains the logic.  
The notebooks let the reader watch that logic unfold.

This is especially important in machine learning education, because many concepts sound simple in prose while remaining poorly understood in practice until one sees a model actually learn, fail, saturate, overfit, collapse, or generalize.

---

## What this project is trying to teach

Across the full repository, the educational objective is not simply to teach names of models. It is to teach how to think about machine learning systems as structured mechanisms.

That means learning to see that:

- a model is a parameterized transformation
- architecture imposes assumptions on data
- optimization shapes behavior but does not guarantee understanding
- better fit is not the same as broader intelligence
- different model families succeed because they encode different forms of inductive bias
- every gain in flexibility comes with tradeoffs in interpretability, efficiency, or data dependence

The project therefore emphasizes not just performance, but explanation. Not just outputs, but processes. Not just definitions, but behavior.

In that sense, **AI-101** is meant to function as a first serious laboratory in machine learning literacy.

---

## The structure of the learning journey

This repository is organized around **10 chapters**, each of which represents a major family of ideas in modern machine learning and artificial intelligence. The sequence is designed to feel cumulative rather than fragmented. Each chapter solves a problem that the previous chapter leaves partially unresolved.

### Chapter 1 — Foundations of Learning Systems

The opening chapter introduces the basic logic of machine learning as learned mapping. It establishes the essential vocabulary of data, parameters, loss functions, optimization, prediction, and generalization. The objective is to build the conceptual floor on which everything else will stand.

### Chapter 2 — Dense Neural Networks

This chapter studies fully connected neural networks as the first substantial parametric function approximators in the sequence. It explains forward propagation, nonlinear activations, backpropagation, and the basic mechanics of gradient-based learning. It also makes clear why dense architectures are powerful yet structurally inefficient for certain classes of data.

### Chapter 3 — Convolutional Neural Networks

This chapter introduces locality, receptive fields, weight sharing, and spatial hierarchy. It shows why convolution transformed machine learning for image-like data and why architectural bias matters. Here the reader begins to see that good model design often comes from respecting the geometry of the data itself.

### Chapter 4 — Recurrent Models and Sequential Structure

This chapter moves from spatial structure to temporal structure. It focuses on sequence modeling, hidden states, information persistence, and the challenge of learning from ordered data. The chapter helps the reader understand both the promise and the fragility of recurrent approaches.

### Chapter 5 — Autoencoders and Representation Learning

This chapter explores compressed representation, latent structure, reconstruction objectives, and the logic of learning meaningful internal encodings. It introduces the idea that a model can learn useful structure even when explicit labels are absent or secondary.

### Chapter 6 — Transformers and Attention

This chapter explains attention as learned routing across a sequence, replacing recurrence with direct relational weighting among elements. It develops the reader’s intuition for token interaction, contextual weighting, and the architectural logic behind modern large-scale sequence models.

### Chapter 7 — Generative Adversarial Networks

This chapter introduces adversarial learning through the interaction of a generator and a discriminator. It demonstrates that learning can take place not only through direct supervised targets, but also through competitive feedback between two models with opposing objectives.

### Chapter 8 — Variational and Probabilistic Deep Learning

This chapter examines uncertainty-aware modeling, latent distributions, and probabilistic interpretations of deep learning systems. It helps the learner move beyond deterministic mappings toward models that acknowledge ambiguity, sampling, and structured uncertainty.

### Chapter 9 — Graph Neural Networks

This chapter shifts the learning setting from grids and sequences to networks of relations. It studies how information propagates across nodes and edges, why graph structure matters, and how non-Euclidean data requires different modeling assumptions from those used in image or text settings.

### Chapter 10 — Evolutionary and Search-Based Learning

The final chapter expands the student’s view beyond gradient descent alone. It studies population-based search, mutation, selection, recombination, and broader optimization logic in settings where gradients may be unavailable, insufficient, or conceptually limiting.

---

## How the book and notebooks relate

This repository is designed so that the book and the notebooks align directly.

Each chapter in the book has a corresponding implementation logic in the notebooks. The book provides conceptual explanation, theoretical framing, and narrative continuity. The notebook provides executable evidence of the chapter’s mechanism.

This dual structure matters because understanding in machine learning is often incomplete if it lives only at one level. Pure theory can become detached from behavior. Pure code can become detached from meaning.

The repository therefore insists on both:

- the conceptual layer
- the executable layer

The reader should be able to move from one to the other without feeling that they are changing subjects.

---

## Recommended way to use this repository

A strong way to work through this repository is the following:

1. Read the relevant chapter material in **/book/** first.
2. Open the corresponding notebook in **/notebooks/**.
3. Run the notebook once exactly as written.
4. Observe the outputs without rushing to judgment.
5. Re-run the notebook while changing one variable at a time, such as sample size, learning rate, hidden width, number of epochs, amount of noise, or model depth.
6. Compare what changes and what remains stable.
7. Write down the mechanism-level lesson before moving on.

The repository is most useful when treated as a laboratory rather than a slideshow. The point is not simply to obtain an answer. The point is to see how the answer came into existence, and what structural assumptions made it possible.

---

## What makes this repository useful for finance and professional learners

Although this repository is not restricted to finance, it is intentionally suitable for **MBA**, **Master of Finance**, and professional practitioner audiences.

That matters because many professional learners do not need maximal theoretical abstraction at the start. They need a serious and disciplined introduction that makes the mechanics of machine learning understandable without turning the subject into vague motivational theater.

For such readers, the value of this repository is that it emphasizes:

- visible mechanism
- clear progression
- conceptual continuity
- runnable experimentation
- failure-aware understanding
- practical intuition without sacrificing rigor

For practitioners in finance, corporate settings, or research functions, this is especially important. Many downstream applications of AI are discussed in strategic language, but strategic language becomes dangerous when it floats free of technical structure. This repository exists to narrow that gap.

---

## Reproducibility and educational discipline

Where possible, the notebooks are built to support repeatable educational outcomes through:

- explicit setup steps
- controlled data generation where appropriate
- fixed seeds when useful
- clear code segmentation
- visible training diagnostics
- plots and intermediate outputs
- a progression from simpler mechanisms to more expressive ones

The point is not to force artificial neatness. The point is to make the learning process inspectable. A student should be able to rerun a notebook, observe the behavior, and explain why the model behaved the way it did.

That is a far more meaningful educational outcome than memorizing a family name like “CNN” or “Transformer” without seeing the operational differences that justify those names.

---

## What this repository is not

This repository is not:

- a production machine learning platform
- a benchmark competition repository
- a claim of commercial superiority
- a substitute for domain validation
- a shortcut around mathematical understanding
- a promise of real-world profitability, predictive dominance, or deployment readiness

It is a **foundational educational repository**.

Its role is to cultivate understanding. That is both more modest and more valuable than pretending every notebook is a product.

---

## Intended audience

This repository is designed for:

- students beginning serious study of machine learning
- MBA and Master of Finance cohorts
- professional practitioners who want technical intuition rather than marketing abstractions
- researchers seeking a compact synthetic teaching environment
- independent learners who prefer mechanisms over slogans

The tone of the project is therefore intentionally clear, structured, and technically respectful. It aims to be accessible without becoming simplistic, and rigorous without becoming performatively obscure.

---

## Repository links

The repository follows this structure:

- **Repository root:**  
  `https://github.com/alexdibol/ai-101`

- **Book folder:**  
  `https://github.com/alexdibol/ai-101/tree/main/book`

- **Notebooks folder:**  
  `https://github.com/alexdibol/ai-101/tree/main/notebooks`

If a compiled book PDF is later placed inside the **/book/** directory, the link will follow this structure:

`https://github.com/alexdibol/ai-101/blob/main/book/<BOOK_FILENAME>.pdf`

If chapter notebooks are named individually, their links will follow this structure:

`https://github.com/alexdibol/ai-101/blob/main/notebooks/<NOTEBOOK_FILENAME>.ipynb`

---

## Educational disclaimer

All materials in this repository are provided for **educational and research purposes only**.

Nothing in this repository constitutes investment advice, trading advice, legal advice, tax advice, accounting advice, audit advice, regulatory advice, or professional certification of any kind.

Any real-world use of machine learning or artificial intelligence systems requires domain-appropriate validation, professional review, and human accountability.

---

## License

This project is released under the **MIT License**.

**Copyright (c) 2026 Alejandro Reynoso**

---

## Contact

**Alejandro Reynoso**  
Email: areynoso@yahoo.com  
GitHub: https://github.com/alexdibol
