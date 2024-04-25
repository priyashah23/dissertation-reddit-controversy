# Detecting Controversy in Reddit
This is a repository dedicated to the code that was created for my dissertation.
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


