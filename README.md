# Automated-Sentiment-Analysis-and-Fake-Review-Detection-and-Rating-Predictions

# Problem Statement
**In today's digital age, online customer reviews have become a crucial aspect of business success, especially for e-commerce platforms and service providers. These reviews provide valuable insights into customer satisfaction, product quality, and service effectiveness. However, the vast volume of reviews makes it challenging for businesses to extract actionable insights manually. Additionally, fake reviews can distort perceptions, making it even harder to gauge genuine customer sentiment. Therefore, there is a need for an automated system to analyze customer reviews, detect fake reviews, and predict customer ratings based on review content.**


# Goals and Objectives
**The overarching objective of this project is to develop an automated, data-driven approach to understanding customer reviews. By analyzing sentiment, detecting fake reviews, and predicting ratings, the project aims to equip businesses with the insights needed to improve customer experiences, make informed decisions, and maintain the integrity of online review systems.**

# The dataset contains the following columns:

-  business_id: ID of the business.
-  date: Date of the review.
-  review_id: Unique ID for the review.
-  stars: Star rating given by the customer (target variable for prediction).
-  text: The review content (feature for predicting ratings).
-  type: Type of entry (all seem to be "review").
-  user_id: ID of the user who posted the review.
-  cool: Coolness score given by other users.
-  useful: Usefulness score given by other users.
-  funny: Funny score given by other users.

# Tools and Technologies
-  **Python Libraries:** NumPy, Pandas, Seaborn, Matplotlib, TextBlob, NLTK, SpaCy
-  **Sentiment Analysis:** VADER, TextBlob, Transformers
-  **Machine Learning:** Scikit-learn, Random Forest, SVM, Logistic Regression, XGBoost
-  **Data Balancing:** SMOTE
-  **Feature Selection:** Recursive Feature Elimination (RFE), VIF
-  **Advanced Techniques:** Gradient Boosting, LightGBM, CatBoost

# Methodology:

-  Data Collection: Gathered customer review data, including review text, star ratings, and other relevant metadata.
-  Data Preprocessing:
--  Cleaned the review text by removing stopwords, special characters, and other unnecessary elements.
--  Performed tokenization, lemmatization, and vectorization using TF-IDF to convert text into numerical format for analysis.
--  Handled missing values, removed duplicates, and balanced the dataset to ensure model stability.
-  Exploratory Data Analysis (EDA):

Analyzed the distribution of customer ratings and review sentiment.
Identified potential patterns and trends within the data using visualizations (e.g., bar plots, word clouds).
Fake Review Detection:

Implemented algorithms to detect potential fake reviews based on features like review length, sentiment, and customer metadata.
Built a classification model to flag suspicious reviews.
Sentiment Analysis:

Used Natural Language Processing (NLP) techniques to analyze the sentiment of customer reviews and categorized them as positive, negative, or neutral.
Model Building:

Split the data into training and testing sets.
Built various machine learning models (e.g., Logistic Regression, Decision Trees, Random Forest, and Support Vector Machines) to predict customer star ratings based on review content.
Evaluated model performance using accuracy, precision, recall, and F1-score metrics.
Model Tuning:

Optimized model hyperparameters using Grid Search and Random Search techniques to improve prediction accuracy.
Model Evaluation:

Compared model performance across different algorithms and identified Random Forest as the best-performing model for rating prediction.


# Conclusion:

**After building various models, the highest accuracy level achieved was 44.1% using the Random Forest model. This indicates that while it's possible to predict customer star ratings based on the content and sentiment of their reviews, the accuracy is limited to 40-45%. As a result, businesses cannot fully rely on these predicted ratings for critical decision-making. However, this model can still be useful for analysis purposes, particularly when ratings are missing, providing a rough estimate for customer satisfaction. While it's not advisable to base decisions solely on predicted star ratings, this automated approach can help in understanding customer sentiment and identifying trends in review data.**
