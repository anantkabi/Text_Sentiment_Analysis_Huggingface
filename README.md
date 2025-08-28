# Pre-requisites and Features
* **Libraries used**: `transformers`, `torch`, `matplotlib`, `pandas`, `collections`
* **Models used**:

  * `distilbert-base-uncased-finetuned-sst-2-english` (binary sentiment: Positive/Negative)
  * `twitter-roberta-base-sentiment-latest` (multi-class: Positive/Neutral/Negative)
* **Features included**:

  * Single sentence sentiment analysis
  * Batch analysis on customer reviews
  * Graph plotting of sentiment results
---

# Text Sentiment Analysis

A simple yet powerful sentiment analysis project built using **Hugging Face Transformers**. This notebook demonstrates how to analyze text sentiment (positive, negative, neutral) using pre-trained transformer models and visualize results with Python.

## 🚀 Features

* Single sentence sentiment detection
* Batch sentiment analysis for customer reviews
* Support for two models:

  * `distilbert-base-uncased-finetuned-sst-2-english` (Positive / Negative)
  * `twitter-roberta-base-sentiment-latest` (Positive / Neutral / Negative)
* Visualizations using Matplotlib

## 📦 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/anantkabi/Text-Sentiment-Analysis.git
cd Text-Sentiment-Analysis
pip install -r requirements.txt
```

Or install manually inside Jupyter:

```python
!pip install transformers torch matplotlib pandas
```

## 🛠️ Usage

1. Open the notebook:

   ```bash
   jupyter notebook Text_Sentiment_Analysis.ipynb
   ```
2. Run the cells to:

   * Load pre-trained models
   * Perform sentiment analysis on sample text
   * Analyze customer reviews in batch
   * Plot results with bar charts

### Example

```python
from transformers import pipeline  

analyzer = pipeline("sentiment-analysis", model="distilbert-base-uncased-finetuned-sst-2-english")  
print(analyzer("I love this project!"))  
# Output: [{'label': 'POSITIVE', 'score': 0.999}]
```

## 📊 Visualization

The notebook includes sentiment distribution graphs to better understand the dataset.

## 📂 Project Structure

```
Text_Sentiment_Analysis.ipynb   # Main notebook
requirements.txt                # Dependencies (to be created)
README.md                       # Project documentation
```

## 🤝 Contributing

Feel free to fork this project and submit pull requests with improvements.

---
