# 📌 NLP Dataset Preparation & Model Fine-Tuning  

## 📖 Overview  
This project demonstrates **Natural Language Processing (NLP)** workflows using the **IMDB Movie Reviews dataset**.  

### Key Features  
- 📂 Dataset selection & preprocessing  
- ✨ Zero-shot classification with **FLAN-T5**  
- 🔧 Fine-tuning & evaluation with **DistilBERT**  
- 🛠 Troubleshooting Hugging Face issues  

---

## 📂 Repository Structure  
NLP-Dataset-Prep/
┣ 📜 NLP_Assignment_Report.pdf # Report/Documentation
┣ 📜 NLP_&_Dataset_Prep.ipynb # Main Jupyter Notebook
┣ 📜 requirements.txt # Required dependencies
┗ 📜 README.md # Project documentation

yaml
Copy
Edit

---

## ⚙️ Setup Instructions  

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/mayank8868/-NLP-Dataset-Prep.git
cd NLP-Dataset-Prep
2️⃣ Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
3️⃣ Run the notebook
Open NLP_&_Dataset_Prep.ipynb in Jupyter Notebook or VS Code and execute cells step by step.

📊 Dataset Details
Source: IMDB Movie Reviews

Classes: Positive / Negative sentiment

Total Size: 50,000 reviews (25k train / 25k test)

Split Used:

90% Training

10% Validation

25k Test

🚀 Models Implemented
🔹 FLAN-T5 (Zero-Shot Prompting)
Uses natural language prompts for classification

No training required

Evaluated on a sample of 200 reviews

🔹 DistilBERT (Fine-Tuned)
Lightweight BERT model fine-tuned on IMDB dataset

Evaluated with accuracy, precision, recall, and F1-score

📈 Results
Model	Accuracy	F1 Score
FLAN-T5 (Zero-Shot, 200 samples)	~0.72	~0.70
DistilBERT (Fine-Tuned)	~0.91	~0.91

🛠 Troubleshooting Notes
⚠️ CUDA Out of Memory → Reduce batch size

⚠️ Tokenizer mismatch → Ensure model & tokenizer checkpoint match

⚠️ Slow training → Enable fp16=True for mixed precision

🙌 Author
👤 Mayank Yadav

