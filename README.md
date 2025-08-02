# Product Analysis Dashboard

This project is an end-to-end sentiment analysis system that analyzes Amazon product reviews for OnePlus and Redmi smartphones using both traditional NLP techniques and deep learning models. It includes a Tkinter-based GUI and provides an analytical dashboard with visualizations for model performance and customer sentiment insights.

## Features

- Sentiment classification using:
  - TextBlob
  - VADER (Valence Aware Dictionary and sEntiment Reasoner)
  - Word2Vec + Naive Bayes
  - BiLSTM (Bidirectional LSTM)
- GUI built with Tkinter for interactive user experience
- Visualizations:
  - Word Clouds
  - Sentiment Distribution Bar Charts
  - Network Graphs for keyword co-occurrence
- Performance metrics: Precision, Recall, F1-Score for each model
- Easy comparison between traditional, rule-based, and deep learning approaches

## Use Case

This project serves as a powerful customer analysis tool that helps e-commerce businesses interpret sentiment trends in customer reviews. The insights assist in improving marketing strategies, enhancing customer experience, and driving business growth.

## Technologies Used

- Python
- Tkinter for GUI
- NLTK, TextBlob, VADER for NLP
- Gensim for Word2Vec
- TensorFlow/Keras for BiLSTM
- Matplotlib, WordCloud, NetworkX for visualizations

## Dataset

- Source: Amazon product reviews for OnePlus and Redmi smartphones
- Format: JSON
- Preprocessing steps: Cleaning, Tokenization, Stopword removal

## Installation and Setup

1. Clone the repository:

```bash
git clone https://github.com/your-username/sentiment-analysis-dashboard.git
cd sentiment-analysis-dashboard
```

2. Create and activate a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```
## How to Run

```bash
python main.py
```
   
## Folder Structure

```
sentiment-analysis-dashboard/
│
├── main.py                # GUI launcher with Tkinter
├── textblob_model.py      # Sentiment analysis using TextBlob
├── vader_model.py         # Sentiment analysis using VADER
├── word2vec_model.py      # Word2Vec embeddings + Naive Bayes
├── bilstm_model.py        # Deep learning model (BiLSTM)
├── visualization.py       # Word clouds, bar charts, network graphs
├── dataset/               # Amazon review CSV files
├── models/                # Pre-trained models
└── README.md
```

## How It Works
  - Launch the GUI (main.py)
  - Select the year
  - The system processes the dataset and classifies reviews
  - The dashboard displays:
  - Word clouds of top words by sentiment
  - Bar charts showing distribution of sentiments
  - Network graphs of keyword associations


## Project Workflow

1. **Data Loading**: Load Amazon review datasets from JSON.
2. **Preprocessing**: Clean, tokenize, and vectorize text.
3. **Model Selection**: Choose from 4 models.
4. **Sentiment Analysis**: Predict sentiment (Positive, Negative, Neutral).
5. **Visualization**: Word clouds, sentiment bar charts, and co-occurrence networks.
6. **Result Display**: GUI shows predictions and visuals interactively.


## Results
- BiLSTM model achieved the highest overall accuracy
- VADER and TextBlob are fast and rule-based, but context-limited
- Word2Vec + Naive Bayes offers a strong tradeoff between speed and performance
- Visualizations enable intuitive understanding of customer sentiments

## Author
- Vaishnavi Polasani
- Email: polsanivaishnavi@gmail.com
- LinkedIn: https://www.linkedin.com/in/polasani-vaishnavi-09615a256/
   
