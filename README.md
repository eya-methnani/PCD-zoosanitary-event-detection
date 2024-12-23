# Automated Zoosanitary Surveillance System in Tunisia

## Project Overview
This project focuses on using advanced Natural Language Processing (NLP) and Machine Learning (ML) techniques to develop an automated system for zoosanitary event detection in Tunisia. It integrates data from multilingual sources such as news outlets and social media to detect the spread of zoonotic diseases, enabling early warnings and timely interventions.

## Key Features
1. **Data Collection and Preprocessing**:
   - Articles were collected in Arabic, French, and English from CNVZ and enriched with web-scraped data.
   - Preprocessing steps include cleaning, tokenization, removal of stop words, stemming, and feature extraction (e.g., TF-IDF, sentiment scores).

2. **Machine Learning Models**:
   - Models trained include Random Forest, SVM, and Logistic Regression using extracted features.
   - Features used: char count, word count, average word length, polarity, and subjectivity.

3. **Large Language Model (LLM)**:
   - Implementation of Multilingual BERT (mBERT) for handling multilingual text.
   - Advanced BERT model with additional numerical and Part-of-Speech (POS) features.

4. **Performance**:
   - Both ML models and LLMs achieved high accuracy, with mBERT slightly outperforming in text understanding.
   - Models were evaluated using metrics such as precision, recall, accuracy, and F1-score.

## Results
- ML Models: High accuracy and effective for structured datasets.
- LLM (mBERT): Superior in handling complex, multilingual text data.
- Custom BERT Model: Integrated linguistic and numerical features for enhanced performance.

## Challenges
- Limited dataset size, necessitating web scraping to balance data.
- Managing multilingual and noisy data for effective training.

## Future Enhancements
- Integration with real-time data sources for faster responses.
- Scaling to process larger datasets and handle more complex scenarios.
- Tailoring LLM models further to meet specific zoosanitary needs.

## Prerequisites
- Python 3.x
- Libraries: `datasets`, `transformers`, `virtualenv`, `plotly`, `BeautifulSoup`


## Usage
1. **Data Preparation**:
   - Place raw data in the `data/raw` directory.
   - Run preprocessing using `preprocess.py`.

2. **Model Training**:
   - Train ML models using `train_ml.py`.
   - Train BERT models using `train_bert.py`.

3. **Evaluation**:
   - Use `evaluate.py` to generate performance metrics and confusion matrices.

## Authors
- **Eya Methnani**  
- **Ghaissen Sebai**

## Supervisors
- **Pr. Anja Habacha**  
- **Dr. Ferihane Kboubi**

---
