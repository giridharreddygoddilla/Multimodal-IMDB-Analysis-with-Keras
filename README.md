# 🎬 Multimodal Movie Genre Prediction using Deep Learning

### 🧠 CNN (Images) + LSTM (Text) | IMDB Dataset | TensorFlow & Keras

<p align="center">
  <img src="https://img.shields.io/badge/Deep%20Learning-CNN%20%7C%20LSTM-ff6f00?style=for-the-badge&logo=tensorflow">
  <img src="https://img.shields.io/badge/Task-Multilabel%20Classification-1e88e5?style=for-the-badge">
  <img src="https://img.shields.io/badge/Dataset-IMDB-43a047?style=for-the-badge">
  <img src="https://img.shields.io/badge/Framework-Keras%20%7C%20TensorFlow-e53935?style=for-the-badge&logo=tensorflow">
</p>

---

## 📌 Project Overview

This project builds a **multimodal deep learning system** to predict movie genres using both:

* 🎥 **Visual features** from movie posters (CNN)
* 📝 **Textual features** from plot summaries (LSTM)

Unlike traditional single-input models, this approach explores how **different data modalities contribute to classification performance**.

> 📊 The project critically evaluates **learning dynamics, convergence behaviour, and precision-recall trade-offs** across models. 

---

## 🎯 Objectives

* Perform **multilabel genre classification** on IMDB dataset
* Compare **CNN vs LSTM performance across modalities**
* Analyse **training behaviour (loss, precision, recall)**
* Identify **model strengths, limitations, and trade-offs**
* Propose **real-world improvements for multimodal systems**

---

## 🧠 Models Implemented

### 🔹 CNN (Image-Based Model)

* Input: Movie posters
* Learns **spatial and visual patterns**
* Architecture: Convolution + Pooling + Dropout

✔ Strong at:

* Visually explicit genres (Action, Animation)
* High precision predictions

❗ Limitation:

* Weak recall for subtle or overlapping genres

---

### 🔹 LSTM (Text-Based Model)

* Input: Plot summaries
* Learns **sequential and semantic relationships**

✔ Strong at:

* Narrative-driven genres (Drama, Biography, Romance)
* Fast convergence and strong generalization

❗ Limitation:

* Struggles with **short / vague descriptions**

---

## 📊 Key Results & Insights

### 📉 CNN Performance

* Training loss reduced from ~0.33 → ~0.21
* Validation loss closely aligned → **no overfitting** 
* Precision reached **~67% (train)** and **~60% (validation)**

👉 Insight:
CNN prioritises **precision over recall**, making it conservative but reliable.

---

### 📉 LSTM Performance

* Rapid convergence (within ~20 epochs)
* Validation loss < training loss → **excellent generalization** 

👉 Insight:
LSTM captures **semantic meaning effectively**, outperforming CNN in narrative genres.

---

### ⚖️ Model Comparison

| Aspect         | CNN (Images)               | LSTM (Text)               |
| -------------- | -------------------------- | ------------------------- |
| Strength       | Visual pattern recognition | Semantic understanding    |
| Precision      | High                       | Moderate                  |
| Recall         | Low                        | Better for text-rich data |
| Generalization | Stable                     | Strong                    |
| Weakness       | Subtle genres              | Short descriptions        |

---

## 🔍 Critical Findings

* 📌 **Precision–Recall Tradeoff**
  CNN performs confident predictions but misses multi-genre signals

* 📌 **Modality Dependency**

  * Visual cues → better for Action/Animation
  * Text → better for Drama/Biography

* 📌 **Model Complementarity**
  Both models solve **different parts of the problem**

👉 This strongly supports **multimodal fusion systems** as the optimal approach

---

## 🚀 Improvements

* 🔹 Replace LSTM with **BERT / Transformers**
* 🔹 Apply **image augmentation** for robustness
* 🔹 Use **fusion models (CNN + LSTM combined)**
* 🔹 Handle imbalance using **focal loss / class weighting**
* 🔹 Add explainability:

  * Grad-CAM (images)
  * Attention maps (text)

---

## 🧰 Tech Stack

* Python
* TensorFlow / Keras
* NumPy / Pandas
* Matplotlib / Seaborn
* GPU Acceleration (Training Optimization)

---

## 💼 Why This Project Stands Out

✔ Combines **Computer Vision + NLP**
✔ Demonstrates **real-world multimodal learning**
✔ Includes **deep evaluation (not just accuracy)**
✔ Shows **critical thinking + model comparison**
✔ Aligns with **industry-level AI systems**

---

## 📌 Conclusion

This project demonstrates that:

* CNN and LSTM individually perform well
* But each has **modality-specific blind spots**
* The future lies in **integrated multimodal architectures**

👉 A combined system would deliver **higher accuracy, better recall, and more balanced predictions**

---

## ⭐ Final Note

This project reflects **end-to-end ML pipeline thinking**, combining:

* Data understanding
* Model building
* Evaluation
* Critical analysis

👉 Designed to meet **real-world AI and industry expectations**
