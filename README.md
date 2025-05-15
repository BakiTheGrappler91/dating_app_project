## 💘 Dating App Naive Bayes Classifier
This project explores natural language processing (NLP) and binary text classification by building a Naive Bayes model to predict whether a dating app user likes or dislikes cats based on the content of their dating profile.
<br/><br/>

### 📌 Project Overview
The goal is to determine if there's a textual pattern that correlates with someone's preference for cats, based on their written dating profile (essay0 field). The result is a machine learning model that classifies profiles into:

Likes cats (label 0)

Dislikes cats (label 1)
<br/><br/>

### 🧠 Key Concepts
- Binary classification using Multinomial Naive Bayes

- Text preprocessing and feature extraction using TF-IDF

- Basic EDA and category encoding

- Model evaluation using confusion matrices, accuracy scores, and classification reports
<br/><br/>

### 🗃️ Dataset
Source: profiles.csv (dating profiles dataset from OKCupid public data)

Key fields used:

- essay0 — user's self-summary text

- pets — used to derive the target label (likes vs. dislikes cats)
<br/><br/>

### 🔍 Workflow Summary
Data Cleaning:

- Remove missing values

- Extract pet preference into a binary label (likes or dislikes cats)

Feature Engineering:

- Use TF-IDF vectorization on the essay text

Model Building:

- Split into train/test sets

- Train a MultinomialNB classifier

Evaluation:

- Accuracy on training and test sets

- Confusion matrix visualizations
<br/><br/>

### 📈 Results
Training Accuracy: ~78%

Test Accuracy: ~33%

⚠️ The drop in test accuracy indicates possible overfitting or lack of predictive signal in the essay text regarding cat preferences.
<br/><br/>

### 📊 Visualizations
Confusion matrix heatmaps for both training and test sets

Axis labels for prediction comparison (actual vs. predicted)
<br/><br/>

### 🔧 Tech Stack
Python

Pandas, NumPy — data manipulation

scikit-learn — modeling, feature extraction, evaluation

Matplotlib, Seaborn — visualizations

TfidfVectorizer — text vectorization

Naive Bayes (MultinomialNB) — classification
<br/><br/>

### 📝 Limitations & Future Improvements
Very low test accuracy suggests text alone is insufficient — could combine with other features (e.g., interests, demographics).

Consider using more advanced NLP models (e.g., logistic regression, SVM, or even transformers).

Add more thorough preprocessing (e.g., lemmatization, spellchecking, stopword removal).

Balance classes if highly imbalanced.
