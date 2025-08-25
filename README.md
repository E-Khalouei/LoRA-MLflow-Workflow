# LoRA-MLflow Workflow

We use the [GLUE/SST-2 dataset](https://www.tensorflow.org/datasets/catalog/glue#gluesst2), based on the Stanford Sentiment Dataset of movie review sentences labeled as positive or negative. 


This is as a learning process for me to learn PEFT specially using LORA  and apply the mlflow. i work with image dataset and text dataset. 
for image dataset, i follow the steps same as https://huggingface.co/docs/peft/en/task_guides/lora_based_methods just i change the data set: https://huggingface.co/datasets/zh-plus/tiny-imagenet and also for process of preaper data for model i remove the aumentation. Note: the hyperparamers doesnt set based on the best value. i just want to the code run fast. to check everything works best.
