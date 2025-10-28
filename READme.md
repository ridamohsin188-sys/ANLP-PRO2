Task 3 — Encoder–Decoder Model (T5) for Text Summarization
Objective

Fine-tune a pre-trained T5 model (t5-small) on the CNN/DailyMail dataset to generate concise summaries for long news articles.

Dataset

Dataset: CNN/DailyMail Summarization Dataset

Train Samples: 287,113

Validation Samples: 13,368

Test Samples: 11,490

Model

Model: t5-small

Framework: Hugging Face Transformers

Tokenizer: T5Tokenizer

Optimizer: AdamW

Training Epochs: 2

Batch Size: 1 (due to GPU memory limits)

Output Directory: /content/t5_summarization

Evaluation Metrics
Metric	Score
ROUGE-1	27.82
ROUGE-2	11.22
ROUGE-L	19.81
ROUGE-Lsum	23.75
Example Outputs

Original:
“Zully Broussard decided to give one of her kidneys to a stranger… resulted in six patients receiving transplants.”

Reference Summary:
“Zully Broussard decided to give a kidney to a stranger. A new computer program helped her donation spur transplants for six kidney patients.”
Model Generated Summary:
“Zully Broussard told CNN affiliate KGO that she was surprised many people benefited. Six recipients received transplants in total.”

Observations

The model captures main ideas well but sometimes repeats phrases (due to small model size).

ROUGE scores are within expected range for t5-small.

Summaries are coherent and concise.

Next Steps

Improve performance by fine-tuning t5-base or t5-large with more epochs.

Add a Gradio app for demo (optional for bonus).

Step 2: README Section for Task 3 (for GitHub)

You can add this to your README.md file:

Task 3: T5 — Text Summarization

Goal: Summarize long news articles from the CNN/DailyMail dataset using a fine-tuned T5 model.

Steps:

Load and preprocess dataset

Tokenize text and summaries

Fine-tune T5-small model

Evaluate with ROUGE metrics

Generate example summaries

Results:

Metric	Score
ROUGE-1	27.82
ROUGE-2	11.22
ROUGE-L	19.81

Example Summary:

“Zully Broussard decided to give a kidney to a stranger. A new computer program helped her donation spur transplants for six kidney patients.”
