# 🛍️ E-commerce Recommender System

A machine learning project to build a personalized product recommendation system for an e-commerce platform using collaborative filtering and matrix factorization. The system helps suggest relevant products to users based on their behavior and preferences.

---

## 🎯 Project Objective

To develop a **Recommender System** that suggests relevant products to users based on:

- Past purchases or ratings
- Behavior of similar users (collaborative filtering)
- Product similarity (via NLP on product descriptions – hybrid approach)

---

## 🧰 Tools & Technologies

- **Python 3**
- **Pandas, NumPy, Scikit-learn**
- **Surprise** (for collaborative filtering)
- **LightFM / SVD** (matrix factorization models)
- **NLTK / spaCy / TF-IDF** (for NLP hybrid model)
- **Streamlit** (optional for UI)

---

## 📁 Dataset

**Source**: [Amazon Electronics Rating Dataset on Kaggle](https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation)

### 📊 Dataset Fields

| Column        | Description                           |
|---------------|---------------------------------------|
| `userId`      | Unique ID of the user                 |
| `productId`   | Unique ID of the product              |
| `Rating`      | Rating given by the user (1-5 stars)  |
| `Timestamp`   | Unix timestamp of interaction         |

---

## 🔍 Project Workflow

### ✅ 1. Data Preprocessing
- Remove duplicates & invalid ratings
- Filter users and items with minimum interactions
- Normalize ratings

### ✅ 2. Modeling Approaches
#### 🔸 Collaborative Filtering
- **User-based**: Recommends products liked by similar users
- **Item-based**: Recommends similar products to what the user liked

#### 🔸 Matrix Factorization
- Using **SVD** or **LightFM** to learn latent features
- Handles sparsity in large-scale datasets

#### 🔸 Hybrid Model (optional)
- Combine collaborative model with **content-based filtering**
- Extract product similarities using **TF-IDF** on product descriptions (if available)

---

## 📈 Model Evaluation

- Precision@K
- Recall@K
- RMSE for rating prediction
- Hit Rate
- Coverage


