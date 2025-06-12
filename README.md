# Finetuning-GPT2

This project demonstrates how to **fine-tune OpenAI's GPT-2** language model using the Hugging Face Transformers library. The notebook walks through the entire process — from data loading and tokenization to training and evaluating the accuracy of the model.

This is useful for creating domain-specific text generation models. 

### **Dataset**

The dataset is loaded from the Hugging Face datasets library. ("mteb/tweet_sentiment_extraction")

Tokenization is done using GPT-2 tokenizer.

### **Finetuning Process**

**Tokenizer & Model Loading**

Load GPT-2 (gpt2) and its corresponding tokenizer.
Resize model embeddings if new tokens are added.

**Dataset Preparation**

Load text and chunk it into blocks of a fixed length.

Tokenize and group texts into training sequences.
Load the dataset

**Train the data**
* Define the training arguments
* Output directory
* Epochs
* Batch size
* Logging steps

**Finetuning Result**

Accuracy after fine-tuning: **70.8%**

The model showed significant improvement over the base GPT-2, especially on domain-specific data.

The generated text was more coherent and relevant to the fine-tuned context.

