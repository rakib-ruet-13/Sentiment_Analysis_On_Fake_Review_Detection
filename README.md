# Impact of Sentiment Analysis in Fake Online Review Detection

![Model Architecture](https://via.placeholder.com/800x300?text=Sentiment+Impact+Pipeline+Diagram)

This repository implements a sentiment-based machine learning framework to detect fake online hotel reviews. The project investigates the effectiveness of integrating **probabilistic sentiment scores** into the fake review classification pipeline.

---

## 📄 Overview

- Develop a **custom sentiment model** trained on hotel reviews.
- Analyze how **sentiment score distributions** vary between truthful and deceptive reviews.
- Improve fake review detection by **replacing binary sentiment labels with probabilistic scores**.

---

## 📦 Dataset

We use the benchmark dataset from [Ott et al. (2013)](http://myleott.com/op-spam.html):

- 800 truthful reviews
- 800 deceptive (fake) reviews  
- Balanced across positive/negative sentiment

> ⚠️ Dataset is not included. Please download it from [here](http://myleott.com/op-spam.html).

---

## 🧪 Key Contributions

- Built a high-accuracy **sentiment classifier** using TF-IDF and Logistic Regression.
- Demonstrated **polarization of sentiment** in deceptive reviews.
- Proposed **probabilistic sentiment integration** for improved fake review detection.

---

## 🔍 Features

| Feature                      | Description                                   |
|-----------------------------|-----------------------------------------------|
| TF-IDF                      | Text vectorization method                     |
| Binary Sentiment Score      | 1 (positive) or 0 (negative) label            |
| Probabilistic Sentiment     | Custom score from sentiment classifier        |
| Final Classifier            | SVM, Logistic Regression                      |

---

## ⚙️ Setup Instructions

```bash
# Clone the repository
git clone https://github.com/rakib-ruet-13/Sentiment_Fake_Review_Impact.git
cd Sentiment_Fake_Review_Impact

# Create virtual environment
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run sentiment classifier
python sentiment_model/sentiment_classifier.py
