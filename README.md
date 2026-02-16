# 📺 YouTube Video Engagement Analytics  
---

## 📌 Project Overview

This project analyzes the **US YouTube Trending Videos dataset (Kaggle)** to understand patterns in video engagement, virality, and content performance.

We explored how video attributes such as:
- Views  
- Likes / Dislikes  
- Comments  
- Title length  
- Tags  
- Publish time  
- Sentiment  

relate to overall engagement and trending behavior.

The analysis combines **EDA, text mining, clustering, and machine learning models** to uncover meaningful engagement insights.

---

## 🎯 Objectives

- Analyze engagement distribution across trending videos  
- Study time-to-trend behavior  
- Examine impact of title length and textual features  
- Segment videos into engagement clusters  
- Build predictive models for viral classification and view estimation  

---

## 📊 Dataset

Source: **Kaggle – YouTube Trending Video Dataset (US)**  

Key Features Used:
- `views`
- `likes`, `dislikes`
- `comment_count`
- `publish_time`, `trending_date`
- `title`, `description`, `tags`
- `category_id`
- `channel_title`

### Engineered Features:
- Engagement Rate  
- Time-to-Trend (hours)  
- Title Length  
- Description Length  
- Sentiment Scores  
- Log-transformed engagement metrics  

---

## 🔍 Methodology

### 1️⃣ Data Preprocessing
- Removed duplicates  
- Converted timestamps  
- Engineered engagement metrics  
- Performed sentiment analysis on text  
- Applied log transformation for skewed distributions  
- 80-20 train-test split  

### 2️⃣ Exploratory Data Analysis (EDA)
- Distribution of views and engagement metrics  
- Correlation analysis  
- Title length vs views  
- Time-to-trend analysis  
- Tag frequency and co-occurrence analysis  

### 3️⃣ Predictive Modeling

#### 🔹 Classification (Viral vs Non-Viral)
Models compared:
- Random Forest ✅ (Best – ~94.6% accuracy)
- XGBoost
- Logistic Regression
- Neural Network

Random Forest achieved highest accuracy and best cross-validation performance.

#### 🔹 Regression (View Prediction)
Random Forest again outperformed other models with:
- Highest R² (~0.94)
- Lowest error metrics

### 4️⃣ Clustering (K-Means)
- Log-transformed engagement features  
- PCA for dimensionality reduction  
- Identified clear high, medium, and low engagement clusters  

---

## 📈 Key Findings

- Engagement metrics are heavily right-skewed  
- Most trending videos gain traction within 24–48 hours  
- Likes and comments strongly predict views  
- Title length has minimal impact on virality  
- Engagement intensity matters more than sentiment direction  
- K-means successfully identified distinct performance segments  

---

## 💡 Recommendations

- Monitor engagement within the first 24–72 hours  
- Focus on total engagement, not just views  
- Optimize titles (40–70 characters recommended)  
- Use relevant, targeted tags  
- Track comment activity as early signal of virality  

---

## 🧠 Conclusion

This project demonstrates how social media analytics, text mining, clustering, and machine learning can uncover actionable insights about online video engagement.

By combining statistical analysis with predictive modeling, we developed a structured framework for understanding what drives trending content on YouTube.

---

