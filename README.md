<div align="center">
  <h1>🌐 Machine Translation & Advanced Document Search System</h1>
  <p><b>(Leveraging Vector Spaces & Locality Sensitive Hashing)</b></p>
  
  [![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)](https://www.python.org/)
  [![NLP](https://img.shields.io/badge/NLP-Machine_Learning-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/Natural_language_processing)
  [![NumPy](https://img.shields.io/badge/NumPy-Power-lightblue?style=for-the-badge&logo=numpy)](https://numpy.org/)
  
  <br>
  <!-- Download Button -->
  <a href="https://github.com/mahmoudamramin/machine-translation/archive/refs/heads/main.zip">
    <img src="https://img.shields.io/badge/⬇️_Download_Project-2EA44F?style=for-the-badge&logo=download&style=flat-square" alt="Download Project" style="height: 45px; border-radius: 8px; margin-top: 15px;"/>
  </a>
</div>

<br>

## 📖 Overview
This project presents a comprehensive, built-from-scratch system that integrates **Machine Translation** and **Advanced Document Search** techniques. Instead of relying on off-the-shelf translation libraries, the project leverages a deep understanding of Word Embeddings and Linear Algebra to bridge different languages. It also addresses the performance bottlenecks in K-Nearest Neighbors (K-NN) searches by implementing advanced **Locality Sensitive Hashing (LSH)**.

---

## 🎯 Goal & Importance in NLP
In modern Artificial Intelligence and Natural Language Processing (such as Large Language Models and RAG applications), **Vector Spaces** and **Embeddings** are foundational concepts. This project highlights their critical importance through two main applications:

1. **Translation as Linear Transformation:**
   - **Significance:** Demonstrates that linguistic meanings can be mathematically represented, and translation can be achieved by finding a Transformation Matrix that projects one language space (e.g., English) into another (e.g., French).
   - **Technique:** Utilizes **Gradient Descent** to minimize the Frobenius Norm, computing the optimal translation matrix with high accuracy.

2. **Fast Approximate K-NN via LSH:**
   - **Significance:** When dealing with massive text datasets (like millions of tweets or documents), traditional linear search methods for calculating distances become impractically slow.
   - **Technique:** Implements **Locality Sensitive Hashing (LSH)** to partition the vector space using hyperplanes, sorting similar texts into common "buckets." This drastically accelerates the retrieval and search process without sacrificing result accuracy.

---

## ✨ Key Features & Technologies
- **Cross-lingual Alignment:** Building a mathematical matrix that projects English word vectors into the French word space.
- **Document Embeddings:** Representing entire sentences or documents (e.g., tweets) by summing up their constituent word vectors using a Bag-of-Words approach.
- **Cosine Similarity:** Precise application of cosine similarity to measure the exact alignment between translated text vectors or queried documents.
- **Advanced Hashing Algorithms (LSH):** Hashing vectors and generating unique IDs using multiple spatial universes to effectively narrow down the search scope.

**Tech Stack:** `Python`, `NumPy`, `NLTK`, `Pandas`, `Jupyter Notebook`.

---

## 📂 Project Structure
The repository consists of the following core components:

```text
📦 Machine-Translation
 ┣ 📜 README.md                 # This documentation file
 ┣ 📓 C1_W4_Assignment.ipynb    # The core notebook of the project (main codebase and model training)
 ┣ 📜 utils.py                  # Advanced helper functions for text preprocessing and similarity math
 ┣ 📜 w4_unittest.py            # Testing suite to ensure the efficiency and correctness of the modules
 ┣ 📂 data/                     # Contains training and testing data (Embeddings & Dictionaries)
 ┗ 📂 images/                   # Illustrative diagrams for vector spaces and the hashing processes
```

---

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mahmoudamramin/machine-translation.git
   cd machine-translation
   ```

2. **Install Dependencies:**
   It is recommended to use a virtual environment. Install the required libraries via pip:
   ```bash
   pip install numpy pandas nltk jupyter
   ```
   *(Note: The code will programmatically download necessary NLTK packages like `stopwords` and `twitter_samples` upon the first run).*

3. **Run the Project:**
   Launch Jupyter Notebook to explore the code and run the system:
   ```bash
   jupyter notebook C1_W4_Assignment.ipynb
   ```

---
<div align="center">
   <i>This project is designed to showcase the immense power of Linear Algebra and Word Embeddings in effectively solving complex Natural Language Processing problems.</i>
</div>
