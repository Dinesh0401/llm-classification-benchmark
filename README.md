# LLM Classification Benchmark 🚀

This repository provides an **automated benchmarking pipeline** to evaluate Large Language Models (LLMs) on **popular text classification datasets** using the OpenAI API.

The framework is designed to be:
- ✅ Fully automated
- ⚡ Asynchronous (fast & scalable)
- 🧠 Dataset-agnostic
- 📊 Accuracy-focused

---

## 🔍 What This Project Does

For each dataset, the script:
1. Automatically downloads the dataset from Hugging Face
2. Detects the input text and label columns
3. Samples a fixed number of examples
4. Dynamically generates a task-specific system prompt
5. Runs multiple LLMs asynchronously
6. Computes classification accuracy
7. Prints consolidated benchmark results

No manual preprocessing. No dataset-specific hacks.

---

## 📚 Supported Task Types

- Binary sentiment classification
- Multi-class topic classification
- Emotion classification
- Intent classification
- Natural Language Inference (NLI)

⚠️ QA and RAG-style datasets (e.g., HotpotQA) are intentionally excluded.

---

## 🧪 Benchmarked Datasets

| Dataset | Task Type |
|-------|----------|
| `stanfordnlp/imdb` | Movie sentiment (binary) |
| `ag_news` | News topic classification |
| `yelp_polarity` | Review sentiment |
| `dbpedia_14` | Entity/topic classification |
| `dair-ai/emotion` | Emotion classification |
| `amazon_polarity` | Product review sentiment |
| `banking77` | Intent classification |
| `snli` | Natural Language Inference |
| `yahoo_answers_topics` | Question topic classification |

All datasets are:
- Public
- Classification-only
- Plug-and-play via Hugging Face

---

## 🧠 Models Evaluated

| Logical Name | Model ID |
|-------------|----------|
| gpt-5.2 | gpt-5.2 |
| gpt-5-mini | gpt-5-mini |

(Replace model IDs if needed.)

---

## ⚙️ How It Works (High Level)

```text
Dataset → Sample → Prompt → Async API Calls → Accuracy → Results
