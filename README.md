 # LoRA-MLflow Workflow (Text dataset)

For the text dataset, I followed the general workflow from:  
- [Kaggle notebook: NLP Fine-Tuning Sentiment Analysis](https://www.kaggle.com/code/yannicksteph/nlp-fine-tuning-sentiment-analysis)  
- [Hugging Face Tokenizer documentation](https://huggingface.co/docs/transformers/en/main_classes/tokenizer)
- [LoRA-based Methods (Hugging Face Docs)](https://huggingface.co/docs/peft/en/task_guides/lora_based_methods)

### 🔧 Key Differences in This Project
- Used the **NSMC Korean dataset** instead of English datasets.  
- Fine-tuned the **`klue/roberta-base`** model.  
- Added **LoRA (Parameter-Efficient Fine-Tuning)** for efficient training.  
- Integrated [**MLflow**](https://mlflow.org/docs/latest/) to save models and track experiments.  

### 📊 Workflow
1. Load dataset (`datasets` library).  
2. Tokenize with Hugging Face `AutoTokenizer`.  
3. Apply LoRA with `peft`.  
4. Train and evaluate with `Trainer`.  
5. Log metrics and models with **MLflow**.


#  Fine-Tuning ViT with LoRA on Tiny-ImageNet

This example follows the Hugging Face PEFT guide; I used the same code (with the augmentation process removed) but with a different dataset (Tiny-ImageNet):  
👉 [LoRA-based Methods (Hugging Face Docs)](https://huggingface.co/docs/peft/en/task_guides/lora_based_methods)



## ⚠️ Notes

- The hyperparameters in this repo are **not optimized for best performance**.  
