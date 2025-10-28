# ANLP-PRO2
ANLP Project — Fine-Tuning NLP Models (BERT, GPT-2, T5)
Overview

This repository contains three NLP tasks for the Advanced Natural Language Processing (ANLP) course.
Each task involves fine-tuning a transformer model from the Hugging Face library to perform a different text-based problem.

 Tasks Summary
Task 1: Emotion Detection (BERT)

Model: bert-base-uncased
Objective: Classify text into emotions — joy, sadness, anger, neutral.
Dataset: Emotion Categories Dataset (Kaggle)

Deliverables:

Preprocessing and tokenization

Fine-tuning with training/validation split

Evaluation metrics: Accuracy, F1-score, Confusion Matrix

Example predictions

Task 2: Recipe Generation (GPT-2)

Model: gpt2
Objective: Generate complete recipes given ingredients or a title.
Dataset: Recipe Dataset (Kaggle)

Deliverables:

Tokenization and dataset formatting

Fine-tuning GPT-2

Evaluation: BLEU, ROUGE, and sample generations

Deployed demo using Gradio

 Live Demo: Gradio App

Task 3: Text Summarization (T5)

Model: t5-small
Objective: Generate concise summaries from long news articles.
Dataset: CNN/DailyMail News Summarization (Kaggle)

Deliverables:

Text preprocessing and summary alignment

Fine-tuning T5

Evaluation with ROUGE metrics

Example summaries
 Technologies Used

Python 3.10+

Hugging Face Transformers

PyTorch

Pandas, NumPy

Scikit-learn

Gradio / Streamlit
How to Run
# Clone the repository
git clone https://github.com/ridamohsin188-sys/ANLP-PRO2.git
cd ANLP-PRO2

# Install dependencies
pip install -r requirements.txt

# Run the Gradio demo (for Task 2)
python app.py

Evaluation
Task	Model	Metric	Result
Task 1	BERT	Accuracy / F1	To be added
Task 2	GPT-2	BLEU / ROUGE	To be added
Task 3	T5	ROUGE-L	To be added
