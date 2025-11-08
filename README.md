## Building a Small LLM from Scratch (Python + PyTorch)

This project walks through the process of **building a tiny GPT-style model from scratch** using PyTorch — a simplified version of a large language model that learns text patterns and generates coherent text. It’s trained on a **streaming dataset from Hugging Face (RedPajama-Data-1T-Sample)**, making it memory-efficient and accessible for anyone learning how large language models actually work under the hood.

## What This Project Does  
	
	- **Data Streaming:** Loads real text data directly from Hugging Face using `datasets`’ streaming API — no downloads needed.  
	- **Tokenization:** Converts raw text into tokens using a custom or SentencePiece tokenizer.  
	- **Model Architecture:** Builds a **Transformer-based GPT mini-model** from scratch (multi-head self-attention, MLP, layer normalization).  
	- **Training Loop:** Trains on small text batches with loss printed at each iteration to show learning progress.  
	- **Text Generation:** Uses a `generate()` function to produce original text from a user prompt.

## Setup  

	You’ll need:  
	- **Python 3.10+**  
	- **PyTorch**  
	- **datasets**, **accelerate**, **sentencepiece**  

	Install dependencies:  
	```bash
	pip install torch datasets accelerate sentencepiece
	```

## How to Run  
	
	1. Open the notebook or script in your IDE (e.g., VS Code, Jupyter).  
	2. Run the code cells in order — it will start training immediately.  
	3. Watch the loss values drop as the model learns to predict the next token.  
	4. After training, try generating text:  

```python
print(generate(model, "The research shows"))
```

**Output Example:**  
```
The research shows that deep models can learn patterns in words and predict new text...
```

## Why This Project Matters  
	
	This project demystifies how GPT-like models are built — from scratch.  
	It’s a hands-on way to understand:  
	- How text is tokenized, embedded, and transformed  
	- How self-attention layers actually function  
	- How models generate coherent text from probabilities  
	- How to **stream and train on massive datasets efficiently**

## Next Steps  

	- Replace the simple tokenizer with **BPE or SentencePiece**  
	- Increase **model size** (layers, heads, or context length)  
	- Train on **larger datasets** for better results  
	- Enable **multi-GPU training** with `accelerate`  

## Tech Stack  

`Python`, `PyTorch`, `datasets`, `accelerate`, `sentencepiece`  
Core concepts implemented: tokenization, embeddings, attention, MLP blocks, and autoregressive text generation.  


## Author  

**Sanjana Waghray** — M.S. Data Science @ Illinois Tech Chicago  
🔗 [sanjanawaghray.com](https://sanjanawaghray.com)  

> “I build systems that help machines learn to think — one token at a time.”  
