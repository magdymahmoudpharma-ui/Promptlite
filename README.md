# PromptLite 🚀

**PromptLite** is an open-source CLI tool and Python library designed to help developers benchmark, optimize, and compress LLM prompts to reduce token usage and latency without losing output quality.

## ✨ Key Features
- **Token Compression:** Automatically trims redundant phrasing while preserving semantic intent.
- **Prompt Benchmarking:** Compare latency, token count, and response consistency across multiple prompt variations.
- **Multi-Model Support:** Works seamlessly with Claude, OpenAI, and local open-weights models.

## 📦 Quick Installation
```bash
pip install promptlite
from promptlite import Optimizer

opt = Optimizer(target_reduction=0.25)
clean_prompt = opt.compress("Your long, verbose system prompt goes here...")
print(clean_prompt)

