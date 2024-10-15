

# Product Recommendation System


## Project Overview

This project implements a personalized product recommendation system for online shopping platform. The system leverages OpenAI's text embedding models to suggest new products to users based on their recently viewed items. By comparing the text embeddings of viewed products with the product database, the system recommends items that align with the user's preferences, enhancing engagement and customer satisfaction.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Model Workflow](#model-workflow)
- [Key Features](#key-features)
- [Results](#results)
---

## Technologies Used

- **Python**: Core programming language for data handling, preprocessing, and system implementation.
- **OpenAI API**: Used for generating text embeddings of product titles and descriptions.
- **NumPy & Pandas**: For data manipulation, handling datasets, and preparing data for analysis.
- **Scikit-learn**: Used for similarity calculations (Cosine Similarity) and PCA (Principal Component Analysis) visualization.
- **Matplotlib & Seaborn**: For visualizing the embeddings, PCA plots, and data insights.
- **Cosine Similarity**: Implemented to measure the similarity between product embeddings for recommendation purposes.
- **Jupyter Notebook**: For code prototyping and interactive development.

---

## Model Workflow

1. **Data Preparation**:
   - Load the product dataset.
   - Combine product titles and descriptions to create rich textual data for embedding extraction.

2. **Text Embedding**:
   - Leverage the OpenAI API to extract text embeddings for both the product dataset and the user’s recently viewed products.
   
3. **Similarity Analysis**:
   - Use cosine similarity from Scikit-learn to compute the similarity between the embeddings of recently viewed products and all products in the dataset.

4. **Recommendation Generation**:
   - Rank products by similarity score and filter out the products the user has already viewed to provide new recommendations.

---

## Key Features

- **Personalized Recommendations**: Provides personalized suggestions to users by analyzing their recent product views.
- **Scalability**: The system can scale with an expanding product catalog, offering relevant recommendations even for large datasets.
- **Text Embedding**: The system uses advanced text embeddings to capture the semantic meaning of product titles and descriptions, improving the relevance of recommendations.
- **Embedding Visualization**: Uses PCA to reduce embedding dimensions and visualize the relationships between products in the recommendation space.

---

## Results

- The recommendation system successfully suggests products that align with users' preferences based on the semantic similarities of product descriptions.
- Embedding visualizations using PCA help understand the structure of the product space, showing clusters of similar items.

---

