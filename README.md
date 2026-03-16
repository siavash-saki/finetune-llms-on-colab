# Open-Source LLMs: A Hands-On Tutorial Series

A practical, beginner-friendly tutorial series for working with open-source language models on [Hugging Face](https://huggingface.co). All notebooks run on **Google Colab's free T4 GPU**.

## Notebooks

| # | Notebook | Topics | Colab |
|---|----------|--------|-------|
| 1 | [Introduction to Hugging Face](01_HuggingFace_Intro.ipynb) | Ecosystem overview, image generation (SDXL-Turbo, SDXL base + refiner), text-to-speech (SpeechT5) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/01_HuggingFace_Intro.ipynb) |
| 2 | [Hugging Face Pipelines](02_HuggingFace_Pipelines.ipynb) | High-level pipeline API, sentiment analysis, zero-shot classification, text generation, NER, table QA, audio, music, image generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/02_HuggingFace_Pipelines.ipynb) |
| 3 | [Hugging Face Tokenizers](03_HuggingFace_Tokenizers.ipynb) | How tokenizers work, encoding/decoding, vocabulary, comparing tokenizers across models (Llama, DeepSeek, Phi, Qwen), model variants, `apply_chat_template` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/03_HuggingFace_Tokenizers.ipynb) |
| 4 | [Model Inference](04_HuggingFace_Model_Inference.ipynb) | Manual inference (tokenizer + model), generation parameters (temperature, top_p, sampling), multiple models (SmolLM3, Phi-4, Llama 3.2, Qwen 2.5), streaming, multi-turn conversations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/04_HuggingFace_Model_Inference.ipynb) |
| 5 | [Quantization](05_HuggingFace_Quantization.ipynb) | float16 vs 8-bit vs 4-bit, `bitsandbytes`, `BitsAndBytesConfig`, NF4, double quantization, running Llama 3.1 8B on a free T4 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/05_HuggingFace_Quantization.ipynb) |
| 6 | [Fine-Tuning with LoRA & QLoRA](06_HuggingFace_FineTuning.ipynb) | Why fine-tune, LoRA and QLoRA explained, dataset preparation, `SFTTrainer`, LoRA configuration, training, saving/loading adapters, before vs after comparison | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/06_HuggingFace_FineTuning.ipynb) |
| 7 | [Tracking, Evaluation & Iteration](07_HuggingFace_TrainingExperiments.ipynb) | Weights & Biases integration, reading training curves, hyperparameter experiments, evaluation strategies, common problems and fixes | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/07_HuggingFace_TrainingExperiments.ipynb) |
| 8 | [Dataset Curation & Advanced Fine-Tuning](08_HuggingFace_AdvancedFineTuning.ipynb) | Dataset formats, building custom datasets, DPO alignment training, merging LoRA adapters, pushing to Hugging Face Hub | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/open-source-LLMs/blob/main/08_HuggingFace_AdvancedFineTuning.ipynb) |

> **Note:** Replace `YOUR_USERNAME` in the Colab links with your GitHub username after pushing the repo.

## Learning Path

The notebooks are designed to be followed in order:

```
Notebooks 1-3: Understanding the fundamentals
  1. What Hugging Face can do (quick tour)
  2. Pipelines (the easy way)
  3. Tokenizers (what happens under the hood)

Notebooks 4-5: Running models with full control
  4. Manual inference, generation parameters, streaming
  5. Quantization (running larger models on limited hardware)

Notebooks 6-8: Fine-tuning your own models
  6. LoRA / QLoRA fine-tuning fundamentals
  7. Experiment tracking, evaluation, and iteration
  8. Custom datasets, DPO alignment, deployment
```

## Prerequisites

- A free [Google Colab](https://colab.research.google.com) account (for GPU access)
- A free [Hugging Face](https://huggingface.co) account (for model access)
- Basic Python knowledge
- For Notebooks 6-8: a free [Weights & Biases](https://wandb.ai) account (for experiment tracking)

## Models Used

Throughout the series, we work with models from several open-source families:

- **SmolLM3** (Hugging Face) — 3B
- **Phi-4-mini** (Microsoft) — 3.8B
- **Llama 3.1 / 3.2** (Meta) — 3B, 8B
- **Qwen 2.5** (Alibaba) — 3B
- **DeepSeek** (DeepSeek AI)
- **SDXL / SDXL-Turbo** (Stability AI) — image generation
- **SpeechT5** (Microsoft), **Bark** (Suno) — audio generation

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
