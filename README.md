# Detecting Controversy in Reddit
This is a repository dedicated to the code that was written for the Individual Literature Review and Project Report. For the project I needed to create three distinct models that used different techniques to attempt to detect controversy in Reddit.  The first model TF-IDF + SVM classifier is a pipeline where the model is split into textual and numerical features. The other two models used embeddings obtained from large language models and used the vector as input in a Multi-Layer Perceptron that classified whether the post was controversial or not. 

This repository contains three notebooks
- TF-IDF+SVM: This file contains all the code related to the pipeline model
- Training_BERT_and_RoBERTa: This file contains all the logic behind extracting embeddings from BERT & RoBERTA model as well as training the model
- finetune-roberta: Is the logic for training the RoBERTa model with a dataset of r/gaming comments.

This repository also contains sample CSV files so that you can attempt to train the data.

In terms of functionality: To get started you will need to update the dataset paths to be the local paths for this repository. 
for example
``` python
df = pd.read_csv("gdrive/MyDrive/Colab Notebooks/Dissertation/cleaned_subreddit_gaming.csv")
```
Would need to be changed to be: 
``` python
df = pd.read_csv("YOUR PATH.csv")
```

## Google Colab Machine requirements to process each model
- TF-IDF+SVM: CPU or a higher model
- Training_BERT and RoBERTA: T4 GPU or a higher model
- Fine-tuning RoBERTA model: A100 GPU or higher

## Libraries
Libraries used in this project included but not limited to: 
- HuggingFace Library (AutoModel, AutoTokenizer, Datasets, Transformers...) 
- Sci-kit Learn Library
- Pytorch Library
- Skorch Library
- Python Reddit API Wrapper (PRAW)
- MatplotLib (Graphs)
- Seaborn (Graphs)
