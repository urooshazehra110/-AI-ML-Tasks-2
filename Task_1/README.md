# News Topic Classification using BERT

## Objective

The objective of this project is to build a News Topic Classification system using a Transformer-based model (BERT). The model classifies news articles into one of four categories:

* World
* Sports
* Business
* Sci/Tech

The project demonstrates the use of transfer learning and transformer fine-tuning for Natural Language Processing tasks.

---

## Dataset

AG News Dataset

The dataset contains news articles belonging to four categories:

| Label | Category |
| ----- | -------- |
| 0     | World    |
| 1     | Sports   |
| 2     | Business |
| 3     | Sci/Tech |

---

## Methodology

### Data Preprocessing

* Combined title and description fields
* Tokenized text using BERT tokenizer
* Applied padding and truncation

### Model Development

* Pre-trained model: bert-base-uncased
* Fine-tuned using Hugging Face Transformers
* Optimizer and training configuration handled through Trainer API

### Evaluation Metrics

* Accuracy
* Weighted F1 Score

### Deployment

The trained model was deployed using Gradio for real-time news classification.

---

## Results

| Metric            | Score |
| ----------------- | ----- |
| Accuracy          | 94%  |
| Weighted F1 Score | 94%  |

The model achieved strong performance across all categories and generalized well to unseen news headlines.

---

## Key Observations

* Transfer learning significantly reduced training time.
* BERT outperformed traditional machine learning approaches for text classification.
* Weighted F1-score closely matched accuracy, indicating balanced performance.

---

## Technologies Used

* Python
* Hugging Face Transformers
* PyTorch
* Scikit-learn
* Gradio
* Google Colab
