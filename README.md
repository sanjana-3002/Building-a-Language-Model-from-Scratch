**Building a Small LLM from Scratch (Python + PyTorch)**

This project shows how to build a tiny GPT-style model from scratch using PyTorch.
It’s a small version of a large language model that can learn simple text patterns and generate new text — all trained on the RedPajama-Data-1T-Sample dataset from Hugging Face.

**What this project does**
	•	Loads real text data directly from Hugging Face using streaming (no downloads needed)
	•	Creates a tokenizer to turn text into numbers the model can understand
	•	Builds a Transformer model step by step (multi-head attention, MLP layers, etc.)
	•	Trains the model on streamed text data
	•	Generates text from a custom prompt


**Setup**

You’ll need:
	•	Python 3.10 or newer
	•	PyTorch
	•	The datasets, accelerate, and sentencepiece libraries

 Install everything with- 
  pip install torch datasets accelerate sentencepiece

How to Run
	1.	Open the project in VS Code or any IDE.
	2.	Run the notebook or script step by step (from top to bottom).
	3.	The model will start training on small text batches and print the loss values as it learns.
	4.	After training, use the generate() function to make the model write text from your prompt.
  5.  Example - print(generate(model, "The research shows"))


**Example -**
  Prompt: The research shows
  Output: The research shows that deep models can learn patterns in words and predict new text...

**Next Steps**

Once you understand this version, you can:
	•	Replace the simple tokenizer with a BPE / SentencePiece one
	•	Increase model size (more layers, heads, or context length)
	•	Train on a bigger dataset
	•	Add GPU/multi-GPU training using accelerate


Why this project is useful

It’s a great starting point to understand:
	•	How GPT-like models work under the hood
	•	How data is tokenized, batched, and trained
	•	How to stream large datasets without storing them locally



Author: Sanjana Waghray

  
