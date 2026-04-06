#  NLP Assignment 5 — POS Tagging & Chunking using Transformers

##  Objective
The goal of this assignment is to build and evaluate transformer-based models for:

- **Part-of-Speech (POS) Tagging**
- **Text Chunking (Shallow Parsing)**

Using modern NLP techniques, we explore how pretrained transformer models like **DistilBERT** can be fine-tuned for token classification tasks.

---

## Learning Outcomes
After completing this assignment, you will be able to:

- Understand **token classification tasks** in NLP
- Differentiate between **POS Tagging and Chunking**
- Apply **transformer-based models (DistilBERT)**
- Handle **subword tokenization alignment**
- Evaluate models using **Precision, Recall, and F1-score**
- Perform **inference on custom text**

---

##  Tools & Technologies

- Python 
- Hugging Face Transformers 
- Datasets / NLTK Corpus
- SeqEval (Evaluation Metrics)
- PyTorch / TensorFlow

---

##  Dataset

- **CoNLL-2000 Dataset** (via NLTK)
- Contains annotated sentences for:
  - POS tagging
  - Chunking (BIO format)

---

##  Project Workflow

### 1️ Dataset Selection
- Used **CoNLL-2000 dataset** from NLTK
- Converted into Hugging Face-compatible format

### 2️ Data Preprocessing
- Tokenization using **DistilBERT tokenizer**
- Handled **subword alignment**
- Applied **-100 masking** for ignored tokens

### 3️ Model Setup
- Model: `DistilBERT`
- Task: `Token Classification`
- Library: Hugging Face Transformers

### 4️ Training
- Trainer API used
- Hyperparameters:
  - Epochs: 3
  - Learning Rate: 2e-5

### 5️ Evaluation
- Metrics:
  - Precision
  - Recall
  - F1 Score
- Library: `seqeval`

### 6️ Inference
- Used `pipeline()` for predictions
- Tested on custom sentences

---

##  POS Tagging vs Chunking

| Aspect | POS Tagging | Chunking |
|---|---|---|
| Level | Word-level | Phrase-level |
| Labels | Flat tags | BIO format |
| Complexity | Low | Medium |
| Context | Local | Contextual |
| Use Case | Grammar | Structure understanding |

---

##  Key Observations

- DistilBERT achieves **high accuracy with fewer parameters**
- Chunking is harder due to **span-level evaluation**
- Transformer models capture **context effectively**
- Transfer learning enables **fast convergence**

---

