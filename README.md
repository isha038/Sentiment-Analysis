# Sentiment-Analysis

This is the link to the dataset: https://www.kaggle.com/code/robikscube/sentiment-analysis-python-youtube-tutorial/input?select=Reviews.csv

## Overview  

This project implements a **Sentiment Analysis Classifier** using two powerful tools:  

1. **VADER** (Valence Aware Dictionary and sEntiment Reasoner) – A rule-based sentiment analysis model.  
2. **RoBERTa** – A pre-trained transformer model from Hugging Face for more advanced NLP tasks.  

It includes quick **Exploratory Data Analysis (EDA)**, as well as polarity scoring using both tools to identify sentiment trends in a dataset.  



## Tools and Libraries  

The following tools and libraries are used in this notebook:  

1. **NLTK**  
   - `SentimentIntensityAnalyzer`: Calculates negative, neutral, and positive sentiment scores.  
2. **Hugging Face Transformers**  
   - **RoBERTa**: A pre-trained transformer-based model for advanced sentiment classification.  
   - Hugging Face **Pipeline**: Simplifies integration of RoBERTa for predictions.  
3. **Python Libraries**:  
   - `Pandas`: Data manipulation  
   - `Matplotlib` / `Seaborn`: Visualizations  
   - `NLTK` and `Transformers`: Sentiment Analysis  


## Key Features  

### 1. **VADER Sentiment Analysis**  
- A **bag-of-words** approach where individual words contribute to the sentiment score.  
- **Key Steps**:  
   1. Stop words (e.g., "and", "the") are removed.  
   2. Each word is scored for polarity (negative/neutral/positive).  
   3. Overall sentiment is calculated for the dataset.  

### 2. **RoBERTa Transformer**  
- Utilizes Hugging Face's **RoBERTa** model for state-of-the-art sentiment analysis.  
- Predictions are obtained using the Hugging Face **Pipeline API** for ease of use.  

-

## Steps Performed  

1. **Data Loading**  
   - Load and preprocess the dataset for sentiment analysis.  

2. **Quick EDA (Exploratory Data Analysis)**  
   - Initial visualizations and checks to understand the dataset.  

3. **VADER Sentiment Analysis**  
   - Analyze sentiment scores (`neg`, `neu`, `pos`) and overall polarity.  

4. **RoBERTa Sentiment Classification**  
   - Perform advanced sentiment analysis using Hugging Face's RoBERTa model.  
   - Compare results with VADER to evaluate accuracy and robustness.  

5. **Visualization**  
   - Visualize sentiment trends and comparisons using bar charts, pie charts, and other plots.  

---

## Requirements  

The following Python libraries are required:  

```bash
pip install pandas matplotlib seaborn nltk transformers torch
```

For NLTK, ensure you have the necessary resources downloaded:  

```python
import nltk
nltk.download('vader_lexicon')
```

---

## How to Run  

1. Clone the repository:  
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Launch Jupyter Notebook:  
   ```bash
   jupyter notebook sentiment_analysis.ipynb
   ```

3. Run the cells sequentially to perform sentiment analysis using both VADER and RoBERTa.  

---


## Results  

- VADER provides quick and interpretable sentiment scores using a **rule-based approach**.  
- RoBERTa delivers more **accurate predictions** leveraging a pre-trained transformer model.  
- Combining both methods enables robust sentiment analysis for various NLP tasks.  

