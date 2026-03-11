# Problem Statement
Modern E-commerce platforms host thousands of products across multiple categories, making it difficult for users to discover items relevant to their interests. Without effective recommendation systems, users may struggle to find suitable products, leading to reduced engagement and lower conversion rates.

# Objective
The objective of this project is to build and evaluate multiple Recommendation Systems to predict products a user is most likely to interact with based on historical interaction data and product attributes.

# Deliverables
- Simulate a realistic e-commerce interaction dataset
- Perform Exploratory Data Analysis (EDA) on user behavior and product interactions
- Implement multiple recommendation algorithms
- Evaluate recommendation performance using Precision@K and Recall@K
- Compare algorithm effectiveness


# 🛍️ E-Commerce Product Recommendation System

An analytics & machine learning project that simulates user-product interactions and builds multiple recommendation algorithms to suggest relevant products to users.

The project evaluates recommendation performance using Precision@K and Recall@K metrics and compares different approaches used in real-world recommendation engines.

---

## 🔧 Tools Used

- Jupyter Notebook
- Python (Pandas, Machine Learning, Numpy, Faker, Scikit-learn, Matplotlib, Seaborn)

---

## 📂 Simulated Dataset

| File | Description |
|-----|-------------|
| `ecommerce_interactions.csv` | Simulated user-product interactions |
| `products.csv` | Product catalog with attributes |
| `users.csv` | Simulated user dataset |

Dataset fields include:

- user_id
- product_id
- category
- brand
- price
- rating
- interaction_type
- interaction_score
- timestamp

---

## 📊 Exploratory Data Analysis

EDA was performed to understand product engagement and user interaction behavior.

Analysis includes:

- Category-wise product interactions
- Top brands by engagement
- Interaction type distribution
- Price distribution
- User activity levels
- Most popular products
- Interaction trends over time

Visualizations were created using **Seaborn and Matplotlib**.

---

## 🧠 Recommendation Algorithms

The following recommendation approaches were implemented.

### 1️⃣ Popularity-Based Model

Recommends products with the highest overall interaction score.

Used as a baseline model.

---

### 2️⃣ Collaborative Filtering

User similarity based recommendation using cosine similarity.

Users with similar interaction patterns are used to recommend products.

---

### 3️⃣ Content-Based Filtering

Recommends products similar to items the user has interacted with.

Product features used:

- category
- brand
- price
- rating

---

## 📏 Model Evaluation

Recommendation models were evaluated using:

### Precision@K Recall@K


Evaluation performed using **K = 5**.

---

## 📈 Model Performance

| Model | Precision@5 | Recall@5 |
|------|-------------|---------|
| Popularity | 0.015 | 0.015 |
| Collaborative Filtering | 0.015 | 0.016 |
| Content-Based Filtering | 0.018 | 0.019 |

---

## 🔍 Key Insights

- Content-Based Recommender performed the best(Precision=0.018, Recall=0.019) and Popularity Recommender the worst(Precision = 0.0.15, Recall = 0.015). This is completely normal for synthetic datasets created with random behavior.
- This dataset was generated using Faker, so user preferences are mostly random. There is no strong pattern for the model to learn.
- Recommendation problems are very sparse which makes the problem very hard to be hard solved unless you have enough and clear data to evaluate on.
- Real-world recommendation systems typically perform better when trained on real behavioral data.On real Streaming or E-commerce platforms like Netflix, Spotify, Flipkart or Myntra; there are millions of users, strong behavioral signals, repeated purchases, clear product clusters. Hence their metrics are higher.

---

## 🙌 Credits

Made with Intent,  
**Shaik Samien Raahhat**
