# Large Language Models (LLMs) - A Comprehensive Guide

Welcome to the **LLMs Project**! This repository is a step-by-step guide to understanding, building, and experimenting with **Large Language Models (LLMs)**, covering everything from basic components to advanced topics like **Retrieval-Augmented Generation (RAG)** and **Chain of Thought (CoT)** prompting.

**Explore more my LLM productions**: websites that allows users to
- Upload pdf files and return information corresponding to questions from users - [Details](https://github.com/HoDangCao/pdf_rag).
- Upload databases, return SQL code and result tables corresponding to user queries within few seconds while
ensuring data security without feeding data to LLMs - [Details](https://github.com/HoDangCao/rag4querydb).

## Table of Contents

1. [**Main Components Overview**](./LLMs_sys_summary.ipynb)
   - What's LLMs?
   - Building a Private LLM
     - Data Curation
     - Data Preprocessing
     - LLM Training
     - Evaluating LLMs
   - RAG (Retrieval-Augmented Generation)
   - Multi-Agent Systems
   - LLMs Quantization

2. [**Building Llama 3 Model**](./Llama/Llama3.ipynb) from scratch
   - Input Block with Byte Pair Encoding (BPE) Tokenizer
   - Decoder Block with Sub-Components:
     - RMS Norm (Root Mean Square Normalization)
     - RoPE (Rotary Positional Encoding)
     - KV Cache
     - Group Query Attention
     - FeedForward Network
   - The Output Block
   - Training & Evaluation
   - Inference Example

3. [**Retrieval-Augmented Generation (RAG)**](./RAG/rag.ipynb)
   - Chunking Data
   - Retrieval Methods: Keyword Based & Vector Embeddings
   - Ranking Retrieved Contexts
   - Evaluation of Retrieved Contexts
   - Augmented Generation Steps
   - Challenges & Solutions in Retrieval
   - Evaluation of RAG

4. [**Chain of Thought (CoT)**](./CoT/CoT.ipynb)
   - Theory of CoT Prompting
   - Properties of CoT Prompting
   - Tree-of-Thought Prompting
   - Reasonings in CoT: Arithmetic, Commonsense, Symbolic
   - Challenges & Limitations
   - Concise CoT
   - Basic Inference Code on CoT Reasoning

5. [**LLM Fine-Tuning Strategies**](./LLM_finetuning.ipynb)
   - Fine-Tuning Process
   - PEFT Techniques: Adapters, Prompt Tuning, Prefix Tuning, LoRA family, IA3, BOFT

---

## 1. Main Components Overview

In this section, you will get a solid foundation of LLMs, their architecture, and the processes involved in building a private LLM:

- **LLMs System Summary**: Learn about the general components that make up an LLM system and what is required to build a private LLM, including **Data Curation**, **Data Preprocessing**, and **LLM Training**.
- **RAG (Retrieval-Augmented Generation)**: Dive deep into how retrieval is integrated with language generation.
- **Multi-Agent Systems**: Explore how multiple LLMs can collaborate to solve tasks.
- **LLM Quantization**: Understand asymmetric and symmetric linear quantization techniques to optimize LLM models.

---

## 2. Building a Llama 3 Model Step by Step

In this section, we take you through the complete process of building and training your own **Llama 3 Model**:

- **Input Block with Byte Pair Encoding (BPE)**: Learn how to preprocess data using BPE to tokenize text efficiently.
- **Decoder Block**: Understand the core components like **RMS Norm**, **RoPE**, and **Group Query Attention**.
- **Training & Evaluation**: Walk through the process of training your model for 40 epochs and evaluating its performance.
- **Inference**: Get hands-on with an example query and response generation.

---

## 3. Retrieval-Augmented Generation (RAG)

RAG combines the power of **retrieval-based** methods with **generation-based** approaches to improve response quality and accuracy:

- **Chunking Data**: Learn how to divide data into manageable pieces for easier retrieval.
- **Retrieval Methods**: Explore both **Keyword-based Retrieval** and **Vector Embeddings** techniques for retrieving relevant data.
- **Ranking Retrieved Contexts**: See how ranking plays a crucial role in selecting the best results.
- **Evaluation of Retrieved Contexts**: Understand how to assess whether retrieved content is valuable.
- **Challenges and Solutions in Retrieval**: Address common obstacles encountered in the retrieval process and how to overcome them.
- **Evaluation of RAG**: Learn how to assess the performance of your RAG system.

---

## 4. Chain of Thought (CoT)

Chain of Thought (CoT) is a powerful technique that enhances LLM reasoning capabilities. This section covers everything you need to know about CoT:

- **CoT Prompting**: Understand how CoT improves reasoning by allowing models to follow a chain of thought.
- **Tree-of-Thought Prompting**: Learn about this variation in CoT prompting and how it extends model capabilities.
- **Reasoning in CoT**: Explore arithmetic, commonsense, and symbolic reasoning methods used in CoT.
- **Concise CoT**: Discover how to streamline CoT to make it more efficient.
- **Inference Code on CoT**: Get hands-on with basic inference code that uses CoT for reasoning.

---

## 5. LLM Fine-Tuning Strategies

Fine-tuning is essential for adapting a pre-trained model to specific tasks. In this section, you will learn the best practices for fine-tuning your LLM:

- **Fine-Tuning Process**: Understand the steps involved in fine-tuning an LLM.
- **PEFT (Parameter-Efficient Fine-Tuning)**: Explore different techniques like **Adapters**, **Prompt Tuning**, **Prefix Tuning**, and **LoRA family** to fine-tune your model efficiently.

---

## How to Contribute

We welcome contributions from everyone! If you have improvements, bug fixes, or new features to add, feel free to fork the repository, create a branch, and submit a pull request.

---

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/HoDangCao/LLMs-System.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Start exploring the notebooks in the **`LLMs_sys_summary.ipynb`** file for the first overview!

---

Happy learning, and we hope you enjoy building LLMs as much as we do! 🚀
