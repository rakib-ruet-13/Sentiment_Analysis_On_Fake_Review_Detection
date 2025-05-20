# Impact of Sentiment Analysis in Fake Online Review Detection

This repository implements a sentimentanalysis based machine learning framework to detect fake online hotel reviews. The project investigates the effectiveness of integrating **probabilistic sentiment scores** into the fake review classification pipeline.

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

Please download it from [here](http://myleott.com/op-spam.html).

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
## Project Structure
```
├── DataSet/ # Contains the original dataset files
│ └── review_data_shuffled # Main shuffled dataset used in training
├── processed_data.csv # Preprocessed version of the dataset
├── processed_dataframe.csv # Additional processed data
├── SMTDFOR.pdf # Published paper
├── LICENSE
├── README.md
├── notebooks/
│ ├── Sentiment_Analysis_Fake_Review_Detection.ipynb (The main file to run run the code)
```

## 🧑‍💻 Authors
Rakibul Hassan — rakibul.hassan@ece.ruet.ac.bd

<a href= 'https://scholar.google.com/citations?user=_UJn9VoAAAAJ&hl=en&oi=ao'> Authors Google Scholar Profile</a>

Md. Rabiul Islam — rabiul.cse@gmail.com

## Citation
If you use this work in your research, please cite the following:
```
@INPROCEEDINGS{9396899,
  author={Hassan, Rakibul and Islam, Md. Rabiul},
  booktitle={2021 International Conference on Information and Communication Technology for Sustainable Development (ICICT4SD)}, 
  title={Impact of Sentiment Analysis in Fake Online Review Detection}, 
  year={2021},
  volume={},
  number={},
  pages={21-24},
  keywords={Support vector machines;Sentiment analysis;Probabilistic logic;Information and communication technology;Electronic commerce;Sustainable development;Business;deceptive online reviews;sentiment analysis;probabilistic sentiment score;logistic regression;TF-IDF;support vector machine},
  doi={10.1109/ICICT4SD50815.2021.9396899}}

```
<a href= 'https://ieeexplore.ieee.org/abstract/document/9396899'> Paper Link  </a>

