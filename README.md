**Movie Recommendation System**

**Overview**

This project implements a **Movie Recommendation System** using both:

* **Collaborative Filtering (KNN)**
* **Content-Based Filtering (TMDB Dataset)**

The system suggests movies based on:

* User rating patterns (Collaborative Filtering)
* Movie features like genres, cast, keywords (Content-Based Filtering)

**Objectives**

* Build a recommendation system using real-world datasets
* Implement both collaborative and content-based approaches
* Compare different recommendation techniques
* Provide accurate and relevant movie suggestions

**Datasets Used**

**MovieLens Dataset (Collaborative Filtering)**

* Contains user ratings for movies
* Features:

  * `userId`
  * `movieId`
  * `rating`

**TMDB Dataset (Content-Based Filtering)**

* Contains movie metadata
* Features:

  * `title`
  * `genres`
  * `keywords`
  * `cast`
  * `crew`
  * `overview`

📥 Dataset Link:
https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

**Technologies Used**

* Python 
* Pandas & NumPy
* Scikit-learn
* Matplotlib & Seaborn
* NLTK (for text processing)
* Google Colab

**Methodology**

**1. Data Preprocessing**

* Handling missing values
* Removing duplicates
* Filtering inactive users and unpopular movies
* Feature extraction from TMDB dataset

**2. Collaborative Filtering (KNN)**

* Created **user-movie matrix**
* Converted to **sparse matrix**
* Applied **K-Nearest Neighbors (KNN)**
* Used **cosine similarity** to find similar movies

**3. Content-Based Filtering**
   
* Combined movie features into a single column (`tags`)
* Applied:

  * Tokenization
  * Lowercasing
  * Stemming
* Converted text into vectors using **CountVectorizer**
* Used **cosine similarity** for recommendations
  
**4. Recommendation System**

* **KNN Model** → recommends based on similar users/movies
* **Content Model** → recommends based on movie similarity

**Exploratory Data Analysis (EDA)**

* Rating distribution histograms
* User activity analysis
* Movie popularity analysis
* Heatmaps for user-movie interactions

**Features**

* Personalized movie recommendations
* Similar movie suggestions
* Efficient computation using sparse matrices
* Handles large datasets

**Limitations**

* Cold-start problem in collaborative filtering
* Lack of personalization in content-based filtering
* Requires data preprocessing and feature engineering

**Future Enhancements**

* Hybrid recommendation system (combine both models)
* Deep learning-based recommendation (Neural Networks)
* Deployment using Streamlit or Flask
* Integration with real-time user data

**How to Run the Project**

1. Upload datasets to Google Drive
2. Open the notebook in Google Colab
3. Mount Google Drive
4. Run all cells sequentially

**Project Structure**

Movie-Recommendation-System/
Datasets/
 movies.csv
 ratings.csv
 tmdb_5000_movies.csv
notebook.ipynb
README.md

**Conclusion**

This project demonstrates how both collaborative and content-based filtering techniques can be used to build an effective movie recommendation system. Each approach has its strengths and limitations, and combining them can further improve recommendation quality.


**Author**

Zagabathuni Udaya Lakshmi
