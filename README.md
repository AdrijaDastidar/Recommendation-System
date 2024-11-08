---

# 🎬 Movie Recommendation System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg) ![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg) ![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Sklearn-brightgreen.svg) ![Neo4j](https://img.shields.io/badge/Neo4j-Knowledge%20Graph-lightblue.svg)

## 📜 Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Approaches](#approaches)
  - [Content-Based Filtering](#1-content-based-filtering)
  - [Collaborative Filtering](#2-collaborative-filtering)
  - [Knowledge Graph-Based Methods](#3-knowledge-graph-based-methods)
  - [Baseline Methods](#4-baseline-methods)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Future Work](#future-work)
- [Contact](#contact)

## 📝 Introduction

This project presents an enhanced **Movie Recommendation System** leveraging multiple algorithms, including **Content-Based Filtering**, **Collaborative Filtering**, and **Knowledge Graphs (KG)**. Traditional recommendation methods often suffer from limitations such as overspecialization and data sparsity. To address these challenges, we have integrated Knowledge Graphs to capture richer and more nuanced relationships between users and movies.

The goal of this system is to provide personalized and diverse movie recommendations by combining user preferences, item metadata, and semantic relationships.

## 📁 Project Structure

```
movie-recommendation-system/
├── Content-Based.ipynb            # Traditional Content-Based Recommendation
├── Correlation.ipynb              # Correlation-Based Recommendation
├── KGBR_Content_Based.ipynb       # KG-Enhanced Content-Based Recommendation
├── KGPR_Collaborative.ipynb       # KG-Enhanced Collaborative Filtering
├── KNN.ipynb                      # K-Nearest Neighbors for Recommendations
├── Weighted-avg.ipynb             # Weighted Average Method
├── README.md                      # Project Documentation
└── Report.pdf                     # Detailed Project Report
```

## 📚 Approaches

### 1. Content-Based Filtering
- Uses movie metadata (genres, cast, etc.) to recommend similar movies.
- Utilizes techniques like **TF-IDF vectorization** and **cosine similarity**.

### 2. Collaborative Filtering
- Based on user-item interactions, recommends movies based on similar users' preferences.
- Addresses data sparsity issues using KG-based relationships between users and items.

### 3. Knowledge Graph-Based Methods
- **Content-Based (KGBR)**: Leverages Knowledge Graphs to capture relationships between movie attributes (like genres, cast, directors).
- **Collaborative Filtering (KGPR)**: Uses Knowledge Graphs to enhance user similarities and movie recommendations by connecting users based on common interactions.

### 4. Baseline Methods
- **K-Nearest Neighbors (KNN)**: Uses item and user features to find nearest neighbors for recommendations.
- **Weighted Average**: Aggregates ratings or similarities based on multiple movie attributes.
- **Correlation**: Uses Pearson correlation for user and item similarity.

## 🛠️ Installation

To run this project locally, follow the steps below:

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Neo4j for Knowledge Graphs

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system
```

### Step 2: Install Dependencies

```bash
pip install numpy pandas scikit-learn neo4j matplotlib
```

### Step 3: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open any of the `.ipynb` files to explore different recommendation approaches.

## 🚀 Usage

1. **Content-Based Recommendations**:
   - Open `Content-Based.ipynb` or `KGBR_Content_Based.ipynb`.
   - Run all cells sequentially to see recommendations based on movie metadata.

2. **Collaborative Filtering**:
   - Open `KGPR_Collaborative.ipynb` to explore KG-enhanced user-based recommendations.

3. **Baseline Comparisons**:
   - Use `KNN.ipynb`, `Weighted-avg.ipynb`, or `Correlation.ipynb` for traditional recommendation techniques.

### Example
```python
input_movie = "Inception"
recommendations = get_recommendations(input_movie)
print(recommendations)
```

## 📈 Results

The models were evaluated using metrics like **Precision**, **Recall**, and **F1-Score**. Here's a summary of the performance:

| Model                  | Precision | Recall | F1-Score |
|------------------------|-----------|--------|----------|
| Content-Based (KGBR)   | 88.4%     | 87.0%  | 87.7%    |
| Collaborative (KGPR)   | 89.2%     | 88.5%  | 88.8%    |
| KNN                    | 82.3%     | 80.5%  | 81.4%    |
| Weighted Average       | 84.1%     | 83.0%  | 83.5%    |
| Correlation-Based      | 80.2%     | 78.9%  | 79.5%    |

The Knowledge Graph-based approaches showed significant improvements over traditional methods in terms of personalization and recommendation relevance.

## 🛠️ Technologies Used

- **Python 3.8+**
- **Jupyter Notebook**
- **Neo4j** for Knowledge Graph construction
- **Pandas & NumPy** for data manipulation
- **Scikit-learn** for machine learning models
- **Matplotlib & Seaborn** for visualizations

## 🔮 Future Work

- Integrate **Hybrid Recommendation Systems** combining both Content-Based and Collaborative Filtering.
- Explore **Deep Learning models** for enhanced feature extraction.
- Extend the Knowledge Graph with additional external data sources (e.g., movie reviews, social media mentions) for even richer recommendations.

## 📧 Contact

For any questions or suggestions, feel free to reach out:
- **Adrija Dastidar** - [adrijadastidar@example.com](mailto:adrijadastidar@example.com)
- GitHub: [AdrijaDastidar](https://github.com/AdrijaDastidar)

---
