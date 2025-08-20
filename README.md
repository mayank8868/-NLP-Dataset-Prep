📌 NLP Dataset Preparation & Model Fine-Tuning
📖 Project Overview

This project demonstrates Natural Language Processing (NLP) workflows using the IMDB movie reviews dataset.
It covers:

Dataset selection and preprocessing

Prompt engineering with FLAN-T5 (zero-shot classification)

Fine-tuning and evaluation with DistilBERT

Troubleshooting common Hugging Face issues

📂 Repository Structure
📦 NLP-Dataset-Prep
 ┣ 📜 NLP_Assignment_Report.pdf   # Report/Documentation
 ┣ 📜 NLP_&_Dataset_Prep.ipynb    # Main Jupyter Notebook
 ┣ 📜 requirements.txt            # Required dependencies
 ┗ 📜 README.md                   # Project documentation

⚙️ Setup Instructions

Clone the repository

git clone https://github.com/mayank8868/-NLP-Dataset-Prep.git
cd NLP-Dataset-Prep


Install dependencies

pip install -r requirements.txt


Run the notebook
Open NLP_&_Dataset_Prep.ipynb in Jupyter Notebook or VS Code and execute cells step by step.

📊 Dataset

Source: IMDB Movie Reviews
 from Hugging Face Datasets

Classes: Positive / Negative sentiment

Size: 25,000 train / 25,000 test reviews

Split: 90% training, 10% validation

🚀 Models Used

FLAN-T5 (Zero-Shot Prompting)

Direct classification using natural language prompts.

DistilBERT (Fine-Tuned)

Lightweight BERT model fine-tuned on IMDB reviews.

Evaluated using accuracy, precision, recall, and F1-score.

📈 Results
Model	Accuracy	F1 Score
FLAN-T5 (Zero-Shot, 200 samples)	~0.72	~0.70
DistilBERT (Fine-Tuned)	~0.91	~0.91
🛠 Troubleshooting Notes

CUDA Out of Memory → Reduce batch size.

Tokenizer mismatch → Ensure tokenizer and model checkpoint match.

Slow training → Use fp16=True for mixed precision.

🙌 Author

👤 Mayank Yadav
