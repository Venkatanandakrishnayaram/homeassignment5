**CRN23848 Neural Networks Deep Learning**

Homework 5

Student Information

Name: Venkata nanda krishna yaram

700765514

**Project Overview:**

This assignment explores Generative Adversarial Networks (GANs), AI ethics topics, basic adversarial simulations, and bias auditing using simple, efficient TensorFlow implementations.

It is divided into the following sections:

GAN Architecture: Explanation and diagram of how GANs work.

Ethics and AI Harm: Analysis of a real-world AI harm scenario and mitigation strategies.

Programming Task: Basic GAN implementation to generate MNIST digits.

Programming Task: Data poisoning simulation on a sentiment classifier.

Legal and Ethical Implications of GenAI: Discussion of memorization and copyright issues.

Bias & Fairness Tools: Study and explanation using the Aequitas Bias Audit Tool.

**Q1: GAN Architecture Explanation:**

Generator's Goal: Create fake data resembling real data.

Discriminator's Goal: Distinguish real vs. fake data.

They compete in a zero-sum game: as one improves, the other must adapt.

Diagram:

pgsql Copy Edit Real Data ----> Discriminator --> Real/Fake? Generated Data (from Generator) --> Discriminator --> Real/Fake?

Generator: random noise → fake data Discriminator: real data OR fake data → classification

Through continuous feedback, both models improve. Eventually, the Generator creates highly realistic data.

**Q2: Ethics and AI Harm Topic Chosen: Misinformation in generative AI.**

Scenario:

A fake news generator system produces realistic yet false political news articles.

Readers are misled during election periods.

Mitigation Strategies:

Verification layers: Incorporate watermarking to identify AI-generated text.

Model filtering: Train models to avoid certain sensitive or false information topics.

**Q3: Programming Task - Basic GAN Implementation:**

Simple GAN trained on MNIST digits.

Generator creates fake images.

Discriminator classifies real vs fake.

Highlights:

TensorFlow + Keras used.

Lightweight training: only 100 epochs.

Sample images saved at Epoch 0, 50, 100.

Loss curves plotted.

**Q4: Programming Task - Data Poisoning Simulation Task:**

Basic sentiment classifier trained on IMDB data.

Introduce poisoning by flipping labels related to "UC Berkeley" reviews.

Evaluate impact on accuracy and confusion matrix.

Highlights:

TensorFlow Sequential model.

Training on small data for quick experiments.

Clear accuracy and confusion matrix comparison before and after poisoning.

**Q5: Legal and Ethical Implications of GenAI Discussion:**

Memorizing private data: Danger of leaking personal information unintentionally.

Copyrighted material generation: Risk of plagiarizing protected works like novels.

Opinion: Yes, generative AI models should be restricted from training on private and copyrighted data. Justification: To respect data privacy, copyright law, and avoid ethical breaches.

**Q6: Bias & Fairness Tools Tool: Aequitas Bias Audit Tool.**

Metric Chosen: False Negative Rate Parity.

Description:

Measures whether different groups have similar false negative rates.

Important to ensure no group is unfairly denied positive outcomes.

Failure Example:

A job application model incorrectly rejects more minority candidates even when qualified.
