# 📧 Spam Email Classifier (SVM + NLP)

A machine learning project that classifies emails as **Spam** or **Ham (Not Spam)** using **Natural Language Processing (NLP)** and **Support Vector Machine (SVM)**.  
The model achieved an accuracy of **98.07%** on the test dataset.



## 📌 Features
- Preprocessing of raw email text for cleaner and more meaningful features.
- Vectorization using **TF-IDF** to convert text into numerical form.
- Classification using **Support Vector Machine (SVC)**.
- High accuracy (**98.07%**) in detecting spam emails.
- Ready to predict on unseen emails.



## ⚙️ Data Preprocessing Pipeline
Before training, the dataset goes through the following preprocessing steps:

1. **Removing duplicated data** → to avoid misleading samples.  
2. **Lowercasing text** → ensures uniformity (e.g., "Spam" and "spam" are treated the same).  
3. **Removing links/URLs** → spam often contains links that can bias the model.  
4. **Removing numbers & punctuation** → keep only meaningful words.  
5. **Removing single characters** → avoids noise like "a", "s", etc.  
6. **Tokenizing text** → split sentences into individual words.  
7. **Removing stopwords** → filter out common words (e.g., "the", "is", "at").  
8. **Lemmatization** → reduce words to their base form (e.g., "running" → "run").  
9. **Re-joining tokens into cleaned strings** → prepare for vectorization.  

After preprocessing, the clean text is transformed using **TF-IDF Vectorizer** and then passed into the **SVM model** for training.



## 🚀 Training Process
1. Load dataset (spam vs. ham emails).  
2. Apply the **NLP preprocessing pipeline** (steps above).  
3. Convert text into numerical features with **TF-IDF**.  
4. Train the model using **SVM (Support Vector Classifier)**.  
5. Evaluate the model on a test set.  




