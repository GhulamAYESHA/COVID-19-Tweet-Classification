# COVID-19-Tweet-Classification
This project applies machine learning techniques to classify COVID-19-related tweets into relevant categories such as Symptoms, Medical Advice, Government Policies, and Personal Experiences. By analyzing social media discussions, Models such as Naïve Bayes, Logistic Regression, LSTMs, and CNNs were implemented and evaluated for performance.

Access Notebook here: https://nbviewer.org/github/GhulamAYESHA/COVID-19-Tweet-Classification/blob/main/covid%2019%20tweet%20classification.ipynb


# 1. Introduction

Social media, especially Twitter, played a significant role during the COVID-19 pandemic, providing critical information and connecting people. However, it also became a source of misinformation. This project focuses on using machine learning models to classify COVID-19 tweets into relevant categories, enabling real-time monitoring and response to public discussions.

# 2. SMART Objectives

- Reduce the gap between training and validation loss by 10% through regularization.
- Implement early stopping to prevent model overfitting.
- Ensure the model generalizes well to new data outside the training set.

# 3. Dataset

The dataset consists of 41,158 English-language tweets manually categorized into five labels: Symptoms, Medical Advice, Government Policies, Personal Experiences, and Others. Preprocessing techniques, such as text normalization and class balancing, were applied to improve data quality for model training.

# 4. Exploratory Data Analysis

An initial analysis revealed an imbalance in class distribution, with certain categories underrepresented. Word frequency analysis showed key terms specific to each category. Topic modeling using LDA helped identify semantic similarities within tweet groups. Location-based metadata analysis indicated the highest tweet activity in the US, followed by the UK and Canada.

# 5. Data Preprocessing

Preprocessing steps included:

- Removing URLs, user mentions, and hashtags.
- Converting text to lowercase and applying lemmatization.
- Removing stopwords and performing n-gram analysis to extract key phrases.

# 6. Model Implementation

Multiple models were evaluated for sentiment classification:

- Naive Bayes: Achieved 46.9% accuracy, with higher recall but limited precision.
- Logistic Regression: Improved accuracy to 61%, providing better classification balance.
- LSTM: Achieved 69.3% accuracy, capturing sequential dependencies in text.
- CNN: Achieved 69.5% accuracy but struggled with long-range dependencies.

# 7. Evaluation

The models were evaluated using precision, recall, and F1-score. LSTM and CNN models outperformed traditional classifiers in capturing sentiment context. However, overfitting was observed in deep learning models, requiring regularization and dropout techniques to improve generalization.

# 8. Conclusion

This project demonstrates that deep learning models, particularly LSTM and CNN, are well-suited for sentiment classification in COVID-19 tweets. While accuracy improvements are possible with additional data augmentation and hyperparameter tuning, Logistic Regression remains a strong baseline model due to its interpretability. Future work involves refining model architectures and incorporating external data sources for enhanced performance.
