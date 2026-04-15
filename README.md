# VisionSearch: Semantic Image Retrieval using CNN vs Transformers

## 🚀 Overview
This project implements a semantic image retrieval system using deep learning.

It compares CNN-based embeddings with Vision Transformer (ViT) embeddings to retrieve visually and semantically similar images from the Caltech101 dataset.

Unlike traditional search methods, this system retrieves images based on visual meaning rather than labels or metadata.

---

## 🧠 Key Idea
Instead of relying on labels, images are converted into feature embeddings.

- Similar images → similar embeddings  
- Dissimilar images → distant embeddings  

Similarity is computed using cosine similarity.

CNN captures **local patterns (textures, edges)**, while Vision Transformers capture **global relationships using attention**, enabling better semantic understanding.

---

## 📂 Dataset: Caltech 101

The project uses the Caltech101 dataset, a widely used benchmark in computer vision.

- ~9,000 images  
- 101 object categories  
- Includes animals, vehicles, instruments, and everyday objects  

This dataset is ideal for evaluating semantic retrieval because of its diverse categories and high variability.

---
## 🏗️ Pipeline

![Pipeline](Pipeline_Semantic.drawio.png)

---
## 🔍 Models Used

### 🧩 CNN-based Feature Extractor
- Pretrained convolutional neural network  
- Captures spatial and local features  
- Strong baseline for image tasks  

### 🔗 Vision Transformer (ViT)
- Splits images into patches  
- Uses self-attention to capture global context  
- Better at understanding semantic relationships  

---

## 📊 Results & Observations

- CNN retrieves images based on **textures and visual patterns**  
- ViT retrieves images based on **semantic meaning**  
- ViT performs better when images differ in background but share the same concept  
- CNN performs well for visually similar images with consistent textures  

---

## 🛠️ Tech Stack

- Python  
- PyTorch  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## ▶️ How to Run

```bash
git clone https://github.com/NiyatiBisht08/visionsearch-cnn-vs-vit
cd visionsearch-cnn-vs-vit

