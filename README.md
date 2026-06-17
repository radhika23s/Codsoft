# Character-Level Neural Text Generation using Stacked LSTM Networks on OpenWebText

## Overview

This project implements a Character-Level Neural Text Generation model using Stacked Long Short-Term Memory (LSTM) networks. The model is trained on a streamed subset of the OpenWebText dataset and learns character-level language patterns to generate new text sequences.

Unlike word-level language models, character-level models predict one character at a time, allowing them to learn spelling, punctuation, sentence structure, and writing patterns directly from raw text. The generated output demonstrates the model's ability to capture linguistic patterns and produce coherent English-like text.

---

## Project Objectives

* Build a character-level language model using deep learning.
* Train a Stacked LSTM network on a large-scale text corpus.
* Learn sequential dependencies between characters.
* Generate human-like text based on a user-defined seed phrase.
* Explore neural text generation techniques used in modern Natural Language Processing (NLP).

---

## Dataset

### OpenWebText Dataset

The project uses a streamed subset of the OpenWebText dataset available through Hugging Face.

OpenWebText is an open-source recreation of the dataset used to train GPT-style language models. It contains high-quality text collected from web pages and articles.

Dataset Source:
https://huggingface.co/datasets/Skylion007/openwebtext

### Dataset Characteristics

* Large-scale web text corpus
* English language content
* Diverse writing styles and topics
* Suitable for language modeling and text generation tasks

For computational efficiency, a subset of the dataset was streamed and processed during training.

---

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Hugging Face Datasets
* Google Colab

---

## Methodology

### 1. Data Collection

The OpenWebText dataset was loaded using the Hugging Face Datasets library in streaming mode to avoid downloading the entire dataset.

### 2. Text Preprocessing

* Combined streamed documents into a single corpus
* Created a unique character vocabulary
* Generated character-to-index mappings
* Converted text into numerical sequences

### 3. Sequence Generation

Input sequences of fixed length were created.

Example:

Input:
Machine learning is amazin

Target:
g

The model learns to predict the next character based on previous characters.

### 4. Model Architecture

The neural network consists of:

* Embedding Layer
* LSTM Layer (128 Units)
* Dropout Layer
* LSTM Layer (128 Units)
* Dropout Layer
* Dense Output Layer with Softmax Activation

### 5. Training

The model was trained using:

* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy
* Batch Size: 128
* Epochs: 10
* Validation Split: 10%

### 6. Text Generation

After training, the model generates text character-by-character using temperature-based sampling to balance creativity and coherence.

---

## Model Performance

### Training Results

| Metric              | Value  |
| ------------------- | ------ |
| Training Accuracy   | 37.15% |
| Validation Accuracy | 38.29% |
| Validation Loss     | 2.1955 |

The decreasing loss and increasing accuracy indicate successful learning of character-level language patterns.

---

## Sample Generated Text

Seed Text:

"The future of technology and machine learning"

Generated Output:

"The future of technology and machine learning ... the model generated coherent word-like sequences, punctuation, and sentence structures by learning patterns from the OpenWebText corpus."

The generated text demonstrates that the model has learned English character distributions, common words, spacing, and writing structure.

---

## Project Structure

```text
Task5_Text_Generation/

├── Text_Generation.ipynb
├── text_generator.keras
├── generated_text.txt
├── README.md
└── screenshots/
    ├── loss_curve.png
    ├── accuracy_curve.png
    └── output.png
```

---

## Future Improvements

* Train on larger subsets of OpenWebText
* Increase model depth and hidden units
* Implement GRU and Transformer architectures
* Fine-tune temperature sampling strategies
* Generate longer and more coherent text passages
* Deploy the model as a web application

---

## Learning Outcomes

Through this project, the following concepts were explored:

* Recurrent Neural Networks (RNNs)
* Long Short-Term Memory Networks (LSTMs)
* Character-Level Language Modeling
* Neural Text Generation
* Sequence Prediction
* Deep Learning for Natural Language Processing

---

## Conclusion

This project successfully demonstrates character-level text generation using a stacked LSTM architecture trained on the OpenWebText dataset. The model learned meaningful language patterns and generated English-like text sequences, highlighting the effectiveness of recurrent neural networks for sequence modeling and text synthesis tasks.

---

