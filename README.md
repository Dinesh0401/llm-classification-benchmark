# LLM Text Classification Benchmark

This repository contains an automated benchmarking script to evaluate Large Language Models (LLMs) on multiple **text classification datasets**.

The benchmark is designed to be:
- Fully automated
- Dataset-agnostic
- Async and rate-limited
- Easy to extend with new datasets or models

---

## 🔍 What This Project Does

- Downloads datasets directly from Hugging Face
- Automatically detects text and label columns
- Samples a configurable number of examples
- Runs LLM inference asynchronously
- Computes classification accuracy
- Produces a consolidated results summary

---

## 📊 Benchmarked Datasets

| Dataset | Task |
|------|------|
| stanfordnlp/imdb | Movie review sentiment (binary) |
| ag_news | News topic classification (4-class) |
| yelp_polarity | Yelp sentiment (binary) |
| dbpedia_14 | Topic classification (14-class) |
| dair-ai/emotion | Emotion classification (6-class) |
| amazon_polarity | Product review sentiment |
| banking77 | Banking intent classification |
| snli | Natural language inference |
| tweet_eval_sentiment | Tweet sentiment |
| yahoo_answers_topics | Topic classification |

---

## ⚙️ Models Evaluated

- gpt-5.2  
- gpt-5-mini  

(Models are configurable in the script.)

---

## 🚀 How to Run (Colab)

1. Open the notebook in Google Colab
2. Set your OpenAI API key in Colab Secrets as:
