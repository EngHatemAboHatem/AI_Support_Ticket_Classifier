# 🤖 Task 5: AI-Powered Support Ticket Categorization (LLMs)

## 📌 Project Overview
Customer service teams handle a massive volume of daily queries. Manually reading and routing these tickets is highly inefficient and time-consuming. This project demonstrates an automated Natural Language Processing (NLP) pipeline that leverages a Large Language Model (LLM) to read customer queries and instantly predict the **top 3 most applicable routing categories**.

## 🗂️ Dataset
The pipeline utilizes the **Banking77** dataset from Hugging Face. This dataset is rich with various banking-related customer service requests, ranging from card delivery issues to top-up failures and transaction disputes.

## 🛠️ Methodology & Technical Approach
Instead of training a model from scratch, this project implements a pre-trained Transformer model (`distilbert-base-uncased-mnli`) using the Hugging Face `pipeline`. Two prompting strategies were implemented and compared:

1. **Zero-Shot Classification:**
   The model categorizes tickets purely based on the semantic meaning of the labels without receiving any prior training examples. It provides a strong, immediate baseline for text categorization.

2. **Few-Shot Learning:**
   We engineered a prompt structure that injects context by providing the model with a few labeled reference examples before asking it to classify a new ticket. This approach effectively steers the model's focus, helping it recognize subtle contexts (e.g., distinguishing between a generic card issue and a specific transaction issue).

## 🚀 Key Takeaways
This implementation highlights the immense potential of LLMs in optimizing customer service operations. By automating the triage process, companies can significantly reduce manual routing time, minimize human error, and ensure much faster response rates for customers.

---
##👤 Author & Organization

Author: Hatem Ali

Student ID: DHC-1079

Organization: DevelopersHub Corporation

**Date:** March 2026
