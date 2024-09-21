
# Sentiment Analysis

This repository contains an implementation of Text Classification (Sentiment Analysis) on the Multilingual Amazon Reviews dataset.

## Requirements
```sh
transformers==4.26.1
tokenizers==0.13.2
datasets==2.10.1
evaluate==0.4.0
wandb==0.13.10

numpy==1.24.2
pandas==1.5.3

```

## Usage

1. Clone the repository: 
```sh
https://github.com/amir7d0/sentiment-analysis.git
```
2. Edit the **`config.py`** file to set the fine-tuning parameters and the dataset to use.
3. Run the training script:
```sh
python finetune.py
```


## Fine-tuning hyperparameters

The following hyperparameters were used during training:

    learning_rate: 2e-05
    train_batch_size: 16
    eval_batch_size: 16
    seed: 42
    optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
    lr_scheduler_type: linear
    num_epochs: 5




You can deploy the model in HuggingFace spaces.
```
git clone https://huggingface.co/spaces/<username>/<space-name>
```

copy src/app.py and src/requirements.txt to the project directory (from GitHub) then commit and push files:

```
!git add app.py
!git add requirements.txt
!git commit -m "Add application file"
!git push
```
