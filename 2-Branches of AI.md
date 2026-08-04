# Branches of AI

**AI**
**Machine Learning**
**Deep Learning**
**Generative AI**

This document explains the main branches of Artificial Intelligence (AI), how they relate to each other, and common applications. Understanding these branches helps you choose the right methods and tools for different tasks and gives context for modern systems such as chatbots, image generators, and recommendation engines.

## Introduction

AI is commonly divided into several overlapping branches: Machine Learning, Deep Learning, and Generative AI. Machine Learning (ML) is the study of algorithms that learn patterns from data to make predictions or decisions. Deep Learning is a subset of ML that uses multi-layer neural networks to learn complex features from large datasets. Generative AI focuses on models that can create new content—text, images, audio, or code—by learning the structure of existing data.

Later in this document we will also discuss Transformer models, which are a key architecture underpinning many modern deep learning and generative models.

---

## Machine Learning

Machine Learning (ML) is a branch of AI that enables systems to learn from data and improve from experience without being explicitly programmed for each task. ML systems learn patterns and relationships in data and then apply those learned patterns to make predictions or decisions on new, unseen data.

Typical ML workflow:
1. Collect and prepare data.
2. Choose or design a model.
3. Train the model on historical data.
4. Evaluate model performance.
5. Deploy the model and use it for inference.

Common applications: recommendation systems (Netflix, YouTube), voice assistants (Siri, Alexa), fraud detection, healthcare analytics, and self-driving cars.

### Types of data

#### Labeled data

Labeled data contains examples paired with the correct output or label. Supervised learning uses labeled datasets so the model can learn mappings from inputs to outputs.

Example: A dataset of images where each image is labeled as "cat", "dog", or "car".

#### Unlabeled data

Unlabeled data has no explicit labels or target values. Unsupervised learning discovers structure in unlabeled datasets.

Example: A large collection of customer transaction records without segment labels.

#### Structured data

Structured data is organized in a fixed schema (tables, CSVs, databases). It is easy to store and query and is often used with traditional ML algorithms.

Examples: tabular datasets, time-series measurements (stock prices, sensor readings).

#### Unstructured data

Unstructured data lacks a predefined schema and includes text, images, audio, and video. Deep learning techniques are commonly used to process unstructured data.

Examples: documents, social media posts, images, recordings.

---

### Supervised learning

Supervised learning uses labeled examples to train models that predict labels for new inputs. It is commonly used for:
- Classification — predicting discrete categories (e.g., spam vs. not spam).
- Regression — predicting continuous values (e.g., house prices).

Typical steps: collect labeled data, split into training/validation/test sets, train a model, tune hyperparameters, and evaluate performance.

Applications: medical diagnosis, credit scoring, image classification, speech recognition.

---

### Unsupervised learning

Unsupervised learning finds patterns and structure in unlabeled data. Common tasks include:
- Clustering — grouping similar items together (e.g., customer segmentation).
- Dimensionality reduction — compressing data while preserving important structure (e.g., PCA, t-SNE).
- Association — discovering rules that describe relationships in data (e.g., market-basket analysis).

Applications: anomaly detection, exploratory data analysis, recommendation systems.

---

### Reinforcement learning

Reinforcement Learning (RL) trains an agent to make a sequence of decisions by interacting with an environment and receiving rewards or penalties. RL is well suited for tasks where actions have long-term consequences.

Key components:
- Agent — the learner or decision-maker.
- Environment — the world the agent interacts with.
- Reward signal — feedback used to reinforce desirable behavior.

Examples: game playing (AlphaGo), robotic control, dialogue systems, and autonomous driving.

---

## Inferencing

Inferencing (inference) is the process of using a trained model to make predictions on new data. This is distinct from training: inference is the deployed, operational use of the model.

Types of inference:
- Batch inference: process large volumes of data at once (e.g., nightly scoring of loan applicants).
- Real-time (online) inference: make predictions immediately as data arrives (e.g., fraud detection during a transaction).
- Edge inference: run models on-device rather than sending data to the cloud (e.g., smart cameras, mobile devices).

Considerations for inference: latency requirements, scalability, cost, privacy, and model size.

Applications: voice assistants, image recognition, fraud detection, recommendation systems, medical diagnosis.

---

## Deep Learning

Deep Learning is a subset of machine learning that uses artificial neural networks with multiple layers (deep neural networks) to model complex patterns in data. Deep models automatically learn hierarchical feature representations from raw input.

How it works (high level): early layers learn simple features (edges in images, short n-grams in text), middle layers combine features into higher-level concepts, and later layers make task-specific predictions.

Advantages:
- Effective on large, complex datasets.
- Learns features automatically, reducing manual feature engineering.
- State-of-the-art performance on many perceptual tasks.

Applications: image and speech recognition, natural language processing, generative modeling, and reinforcement learning when combined with deep networks.

### Main architectures

- Artificial Neural Networks (ANN): the general family of feed-forward networks for prediction and classification.
- Convolutional Neural Networks (CNN): specialized for grid-structured data like images; excel at object detection and image classification.
- Recurrent Neural Networks (RNN) and variants (LSTM, GRU): designed for sequential data such as time series or text (historically popular for language tasks until transformers became dominant).
- Transformer models: attention-based architecture that has become the standard for many NLP and multimodal tasks.
- Generative Adversarial Networks (GAN): models that can generate realistic new data by pitting a generator and discriminator against each other.

---

## Computer Vision

Computer Vision is the field that enables machines to interpret and understand visual data (images and video). Modern computer vision relies heavily on deep learning techniques (especially CNNs and transformers).

Examples: face recognition, object detection, image segmentation, medical imaging analysis, and autonomous vehicle perception.

---

## Natural Language Processing (NLP)

Natural Language Processing enables computers to understand, interpret, and generate human language. Modern NLP uses deep learning and transformer models to perform tasks such as:
- Text classification (sentiment analysis, spam detection)
- Named entity recognition
- Machine translation
- Question answering and summarization
- Text generation (chatbots, writing assistants)

NLP pipelines often include tokenization, embedding (converting words/tokens to vectors), encoding (contextual understanding via models), and decoding (generating outputs).

---

## Generative AI

Generative AI refers to models that create new content similar to the data they were trained on. These models can produce text, images, audio, video, and even structured data or program code.

Common generative models and examples:
- Autoregressive language models (e.g., GPT family) — generate text one token at a time.
- Diffusion models (e.g., DALL·E 2, Stable Diffusion) — generate images by reversing a noising process.
- Generative Adversarial Networks (GANs) — used for high-quality image synthesis and style transfer.

Popular examples and tools: ChatGPT, Microsoft Copilot, Google Gemini, DALL·E, Midjourney, and Stable Diffusion.

Benefits: speed, productivity, creative assistance, and automation of routine content generation.

Limitations and risks: hallucinations (incorrect or fabricated outputs), bias in training data, copyright and ownership concerns, privacy issues, and the need for careful human oversight.

Best practices: verify outputs, use human-in-the-loop workflows, apply content filtering, and ensure clear attribution and transparency where appropriate.

---

## Conclusion

The branches of AI—Machine Learning, Deep Learning, and Generative AI—provide complementary approaches for building intelligent systems. Machine Learning offers general-purpose algorithms for prediction and pattern discovery. Deep Learning provides powerful tools for learning from unstructured data and complex patterns. Generative AI enables systems to create new, useful content. Together these fields power many modern applications, and understanding their differences helps practitioners choose the right approach for a given problem.
