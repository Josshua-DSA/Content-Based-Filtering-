# Content-Based-Filtering Music Recommendation System

A simple music recommendation system using content-based filtering techniques to suggest songs based on musical attributes and metadata similarities.

## 🎯 Overview

This project implements a content-based filtering recommendation system for Indonesian music tracks. The system analyzes song features including genre, artist, album, release year, and popularity metrics to generate personalized music recommendations using TF-IDF vectorization and cosine similarity calculations.

## 🚀 Features

- **Content-Based Filtering**: Recommends music based on song attributes and metadata
- **TF-IDF Vectorization**: Utilizes Term Frequency-Inverse Document Frequency for feature extraction
- **Cosine Similarity**: Calculates similarity scores between songs for accurate recommendations
- **Multi-Genre Support**: Handles various music genres including indie, pop, rock, and reggae
- **Performance Evaluation**: Includes evaluation metrics to assess recommendation quality
- **Interactive Interface**: Easy-to-use functions for generating and displaying recommendations

## 🛠️ Technical Specifications

- **Environment**: Jupyter Notebook
- **Python Version**: 3.12.5
- **Core Libraries**:
  - pandas - Data manipulation and analysis
  - numpy - Numerical computing
  - scikit-learn - Machine learning algorithms and metrics
  - TfidfVectorizer - Text feature extraction
  - cosine_similarity - Similarity calculations
  - StandardScaler - Feature normalization

## 📊 Dataset Structure

The system works with a music dataset containing:
- **Song Title**: Track names
- **Artist**: Performer information
- **Album**: Album details
- **Views**: Popularity metrics
- **Release Year**: Temporal information
- **Genre**: Musical category classification

**Dataset Size**: 161 songs across 4 genres from 71 unique artists (1993-2025)

## 🔧 System Architecture

### 1. Data Loading & Preprocessing
- Dataset import and initial exploration
- Feature combination and normalization
- Text preprocessing with Indonesian stopwords

### 2. Feature Engineering
- TF-IDF matrix generation for combined features
- Numerical feature standardization
- Feature vector creation for similarity calculations

### 3. Similarity Computation
- Cosine similarity matrix calculation
- Similarity score ranking and sorting
- Top-N recommendation selection

### 4. Recommendation Engine
- Song-based recommendation function
- Configurable recommendation count
- Detailed recommendation metadata

## 📈 Performance Evaluation

The system includes evaluation metrics to assess recommendation quality:
- **Genre Consistency**: Measures same-genre recommendation accuracy
- **Success Rate**: Calculates percentage of relevant recommendations
- **Similarity Scores**: Quantifies recommendation relevance

## 🚀 Usage

### Basic Recommendation
```python
# Get recommendations for a specific song
show_recommendations('Semua Aku Dirayakan', num_rec=5)
```

### Custom Recommendation Function
```python
# Generate recommendation list
recommendations = recommend_songs('Song Title', num_rec=10)
```

## 📋 Installation Requirements

```bash
pip install pandas numpy scikit-learn jupyter
```

## 🎯 Key Functions

- `recommend_songs()`: Core recommendation algorithm
- `show_recommendations()`: Display formatted recommendations
- `evaluate_genre_similarity()`: Performance evaluation
- Data preprocessing and feature engineering utilities

## 🔍 Results

The system demonstrates high accuracy in genre-based recommendations with:
- **100% success rate** for same-genre recommendations in testing
- Effective similarity scoring using cosine similarity
- Comprehensive metadata preservation in recommendations

## 🌟 Future Enhancements

- Advanced feature engineering with audio characteristics
- Hybrid recommendation combining collaborative and content-based filtering
- Real-time recommendation updates
- Enhanced evaluation metrics and cross-validation
- Integration with music streaming APIs
  

*Developed using Jupyter Notebook with Python 3.12.5 kernel*
