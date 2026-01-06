# Task 2 part 2: Auto Tagging Support Tickets Using LLM

## 📌 Problem Statement & Objective
The goal of this task was to automate the classification of customer support tickets. Instead of training a model from scratch, we utilized **Zero-Shot Learning** with a Large Language Model (LLM) to classify text into categories without needing a labeled training dataset.

## ⚙️ Methodology
1.  **Model Selection:** We used `facebook/bart-large-mnli`, a powerful model pre-trained on the Multi-Genre Natural Language Inference (MNLI) corpus.
2.  **Zero-Shot Classification:** We defined a list of candidate labels (Technical Issue, Billing, etc.) and asked the model to assign the most probable tag to each ticket.
3.  **Dataset:** Created a representative dataset of support tickets to test the model's capabilities.

## 📊 Key Results
* **Accuracy:** The model achieved **83.33% accuracy** on the test set.
* **Performance:** It correctly identified technical issues, returns, and shipping inquiries without any prior fine-tuning on specific data.

## 🛠 Tools Used
* Python
* Hugging Face Transformers (`pipeline`)
* Pandas
