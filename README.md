# 📝 Task-04: Sentiment Analysis & Visualization  

## 📌 Overview  
This project analyzes and visualizes **sentiment patterns in text data** to understand public opinion and attitudes.  
For this task, the **NLTK Movie Reviews dataset** was used (built into NLTK). It contains **positive** and **negative** movie reviews.  

We applied **lexicon-based sentiment analysis** techniques (VADER & TextBlob) and compared their predictions against the true labels. The project also includes **data visualization** to explore sentiment distributions and word usage.  

---

## 📂 Dataset  
- **Source**: [NLTK Movie Reviews Corpus](https://www.nltk.org/nltk_data/)  
- **Classes**:  
  - `pos` → Positive reviews  
  - `neg` → Negative reviews  
- **Size**: 2,000 reviews (1,000 positive, 1,000 negative)  

---

## ⚙️ Steps Performed  
1. **Data Loading**  
   - Loaded `movie_reviews` dataset from `nltk.corpus`.  

2. **Data Preprocessing**  
   - Lowercased text, removed punctuation, numbers, and stopwords.  
   - Tokenized reviews for word-level analysis.  

3. **Sentiment Analysis**  
   - Used **VADER SentimentIntensityAnalyzer** to compute polarity scores.  
   - Applied **TextBlob** for polarity & subjectivity scores.  
   - Classified texts into **positive, negative, or neutral**.  

4. **Visualization**  
   - Distribution of true labels vs predicted sentiments.  
   - Histograms of polarity scores.  
   - Boxplots (compound score vs true label).  
   - WordClouds for **positive** and **negative** reviews.  
   - Top frequent words in each class.  
   - Confusion matrix comparing predicted vs actual labels.  

5. **Evaluation**  
   - Generated classification reports and confusion matrices.  
   - Measured accuracy of lexicon-based approaches vs ground truth.  

---

## 📊 Results & Insights  
- **VADER** works fairly well for classifying reviews, but sometimes mislabels long/complex sentences.  
- **Positive reviews** commonly use words like *great, wonderful, love, excellent*.  
- **Negative reviews** highlight terms like *bad, boring, waste, worst*.  
- Average polarity from TextBlob and VADER confirms overall dataset balance (equal pos/neg).  

---

## 🛠️ Technologies Used  
- **Python** 🐍  
- **NLTK** – Movie Reviews Dataset, Tokenization, VADER  
- **TextBlob** – Polarity & Subjectivity Analysis  
- **Pandas & NumPy** – Data Handling  
- **Matplotlib & Seaborn** – Visualization  
- **WordCloud** – Word clouds for positive & negative reviews  
- **Scikit-learn** – Confusion Matrix, Classification Report  

---


