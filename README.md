# Word-Similarity-using-Deep-Learning
nlp, word-embeddings, skip-gram, tensorflow , natural-language-processing

This corpus helps the model learn relationships like:
- king ↔ queen  
- king ↔ man  
- queen ↔ woman  

---

## ⚙️ Project Workflow

### 1️⃣ Text Preprocessing
- Tokenize text using Keras `Tokenizer`
- Convert words into integer indices
- Build word-to-id and id-to-word mappings

### 2️⃣ Training Data Generation
- Generate **(target, context)** word pairs using Keras `skipgrams`
- Apply **negative sampling**
- Prepare labels for binary classification

### 3️⃣ Model Architecture
- Two input layers (target word & context word)
- Shared **Embedding layer**
- Dot product to measure similarity
- Sigmoid output for binary classification

### 4️⃣ Model Training
- Loss: Binary Crossentropy
- Optimizer: Adam
- Trained for 50 epochs

### 5️⃣ Embedding Extraction
- Extract learned word vectors from the embedding layer

### 6️⃣ Evaluation
- Measure semantic similarity using **cosine similarity**
- Example comparisons:
  - king vs man
  - king vs queen
  - king vs strong

---

## ✅ Sample Results
The trained model produces higher similarity scores for semantically related words, showing that embeddings successfully capture word meaning.

---

## 🎯 Purpose of This Project
This project is intended for:
- Learning how word embeddings work
- Understanding Skip-Gram architecture
- Practicing TensorFlow Keras Functional API
- Demonstrating core NLP concepts in a simple and interpretable way

---

## 📌 Future Improvements
- Use a larger real-world corpus
- Increase embedding dimensions
- Visualize embeddings using t-SNE or PCA
- Implement CBOW model
