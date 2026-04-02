# GPT-2 Sentiment Classification with LoRA Fine-Tuning

## Project Overview
Fine-tuned GPT-2 on the Amazon Reviews Multi (English) dataset using Parameter-Efficient Fine-Tuning (PEFT) with LoRA (Low-Rank Adaptation) for binary sentiment classification.

## Results
| Model | Accuracy |
|-------|----------|
| Original GPT-2 (baseline) | 44% |
| Fine-Tuned GPT-2 (LoRA) | 78% |
| **Improvement** | **+34%** |

## Tech Stack
- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face PEFT (LoRA)
- Amazon Reviews Multi dataset (mteb/amazon_reviews_multi)

## Project Steps
1. Loaded pre-trained GPT-2 and evaluated baseline performance
2. Applied LoRA fine-tuning using Hugging Face PEFT library
3. Trained on English Amazon Reviews (binary: positive vs negative)
4. Evaluated and compared fine-tuned model against baseline

## LoRA Configuration
- Rank (r): 16
- Alpha: 16
- Dropout: 0.05
- Target modules: c_attn (attention layers)

  ## About
Completed as my final project to the Accenture LearnVantage x Girls Who Code Generative AI Fundamentals program (Udacity).
