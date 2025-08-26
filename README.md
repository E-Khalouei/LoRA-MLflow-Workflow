# LoRA-MLflow Workflow

We use the [GLUE/SST-2 dataset](https://www.tensorflow.org/datasets/catalog/glue#gluesst2), based on the Stanford Sentiment Dataset of movie review sentences labeled as positive or negative. 


This is as a learning process for me to learn PEFT specially using LORA  and apply the mlflow. i work with image dataset and text dataset. 
for image dataset, i follow the steps same as https://huggingface.co/docs/peft/en/task_guides/lora_based_methods just i change the data set: https://huggingface.co/datasets/zh-plus/tiny-imagenet and also for process of preaper data for model i remove the aumentation. 

 # LoRA-MLflow Workflow (Text dataset)

For the text dataset, I followed the general workflow from:  
- [Kaggle notebook: NLP Fine-Tuning Sentiment Analysis](https://www.kaggle.com/code/yannicksteph/nlp-fine-tuning-sentiment-analysis)  
- [Hugging Face Tokenizer documentation](https://huggingface.co/docs/transformers/en/main_classes/tokenizer)  

### 🔧 Key Differences in This Project
- Used the **NSMC Korean dataset** instead of English datasets.  
- Fine-tuned the **`klue/roberta-base`** model.  
- Added **LoRA (Parameter-Efficient Fine-Tuning)** for efficient training.  
- Integrated **MLflow** to save models and track experiments directly in Google Colab.  

### 📊 Workflow
1. Load dataset (`datasets` library).  
2. Tokenize with Hugging Face `AutoTokenizer`.  
3. Apply LoRA with `peft`.  
4. Train and evaluate with `Trainer`.  
5. Log metrics and models with **MLflow**. 


## ⚠️ Notes

- The hyperparameters in this repo are **not optimized for best performance**.  
