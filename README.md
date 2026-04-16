# 🧠 Mental Health Classification using BERT with Temporal Sentiment Tracking

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-BERT-red)
![NLP](https://img.shields.io/badge/NLP-Mental%20Health-green)
![Status](https://img.shields.io/badge/Project-Research-blueviolet)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Description

This project presents a **transformer-based Natural Language Processing system** for detecting mental health conditions from social media text. The model uses a **fine-tuned BERT architecture** to classify posts into multiple psychological states including anxiety, depression, stress, suicidal ideation, personality disorders, bipolar disorder, and normal behavior.

Beyond classification, the project introduces **temporal sentiment tracking**, which visualizes how a user's mental state evolves across multiple posts. This allows the system to identify **patterns and transitions in emotional states**, offering insights that can support early detection of mental health deterioration.

The proposed model achieves **82.2% classification accuracy** on a multi-class Reddit dataset and demonstrates the effectiveness of transformer-based models for mental health monitoring.

---

## 🧩 Key Features

* Multi-class **mental health classification using BERT**
* Detection of **7 mental health categories**
* **Temporal sentiment tracking** for mood progression
* **Confusion matrix & evaluation metrics**
* Lightweight **frontend visualization**
* Training performed using **HuggingFace Transformers**

---


## 📊 Model Performance

**Overall Accuracy:** 82.2%

| Class                | Precision | Recall | F1   |
| -------------------- | --------- | ------ | ---- |
| Anxiety              | 0.86      | 0.86   | 0.86 |
| Bipolar              | 0.88      | 0.80   | 0.83 |
| Depression           | 0.79      | 0.76   | 0.77 |
| Normal               | 0.95      | 0.95   | 0.95 |
| Personality Disorder | 0.67      | 0.71   | 0.69 |
| Stress               | 0.74      | 0.67   | 0.70 |
| Suicidal             | 0.70      | 0.76   | 0.73 |

---

## 🧪 Dataset

The dataset used in this project is **Combined Data.csv**, a public dataset available on Kaggle containing labeled Reddit posts related to mental health discussions.

* Total Samples: **15,800+**
* Source: **Reddit**
* Multi-class labels representing different psychological states

Synthetic **user IDs and timestamps** were generated to simulate user behavior for temporal sentiment tracking.

---

## 🧠 Model Architecture

```
Input Text
   │
Preprocessing
   │
BERT Tokenizer
   │
BERT Encoder (12 Transformer Layers)
   │
Dropout Layer
   │
Dense Classification Layer
   │
Softmax Output
   │
Mental Health Label
```

---

## 📈 Temporal Sentiment Tracking

To extend classification results, the project includes **time-series visualization of predictions**.

This enables:

* Monitoring emotional progression
* Detecting behavioral trends
* Identifying potential mental health deterioration

Example patterns include:

* Anxiety → Depression transitions
* Stress fluctuations
* Sudden spikes indicating suicidal risk

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/mental-health-bert.git
cd mental-health-bert
```

Install dependencies:

```bash
pip install transformers torch pandas numpy scikit-learn matplotlib seaborn
```

---


---

## Training Details

| Parameter     | Value                            |
| ------------- | -------------------------------- |
| Model         | BERT-base-uncased                |
| Optimizer     | AdamW                            |
| Learning Rate | 2e-5                             |
| Batch Size    | 8                                |
| Epochs        | 3                                |
| Loss Function | Cross-Entropy with class weights |

---

## Evaluation Metrics

Model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### Classification Performance

| Class                | Precision | Recall | F1   |
| -------------------- | --------- | ------ | ---- |
| Anxiety              | 0.86      | 0.86   | 0.86 |
| Bipolar              | 0.88      | 0.80   | 0.83 |
| Depression           | 0.79      | 0.76   | 0.77 |
| Normal               | 0.95      | 0.95   | 0.95 |
| Personality Disorder | 0.67      | 0.71   | 0.69 |
| Stress               | 0.74      | 0.67   | 0.70 |
| Suicidal             | 0.70      | 0.76   | 0.73 |

Overall Accuracy: **82.2%**


---

## Running the Model

Open the training notebook in **Google Colab or Jupyter Notebook** and execute the training pipeline.

The notebook performs:

1. Data loading
2. Preprocessing
3. BERT fine-tuning
4. Evaluation
5. Prediction generation
6. Temporal visualization

---

## Results

The fine-tuned BERT model demonstrates strong performance in detecting mental health indicators from text while maintaining good generalization across classes.

Key findings:

* High accuracy for **Normal and Anxiety classes**
* Moderate performance for **Depression and Stress**
* Challenges remain in detecting **rare classes like Personality Disorder**

The addition of **time-series tracking** provides deeper insight into mental health trajectories rather than static classification.

---

## Future Work

Possible improvements include:

* Incorporating larger and multilingual datasets
* Applying **class imbalance correction techniques**
* Deploying the model as a **web application**
* Integrating **real user timeline data instead of synthetic timestamps**
* Extending to **multimodal signals (text + behavioral patterns)**

---

## Contributors

* Hemasri Sanchula
* Keathan Singh
* Lahari
* Project developed as part of research in **AI-based mental health analysis**

---

## License

This project is intended for **research and educational purposes only**.

---

