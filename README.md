# Saudi-Dialect-GPT
This project includes:
1- Building a GPT2 from scratch

2- Training a GPT2 tokenizer on Saudi raw data (tweets)

3- Applying SFT to the pre-trained model, training it to answer in a Saudi dialect. 

## Contents
1. [Data Preparation](#Data-Preparation)
2. [Toknization](#Toknization)
3. [Training](#Training)
4. [SFT data Preparation](#SFT-data-Preparation)
5. [SFT to the pre-trained model](#SFT-to-the=pre-trained-model)
6. [Evaluation](#Evaluation)
7. [Results](#Results)

## Data Preparation
The dataset used to pre-train the GPT2 model from scratch was Saudi dialect tweets. This dataset was obtained from the [figshare website](https://figshare.com/articles/dataset/Saudi_tweets_dataset/6983006?file=12808310). It is a raw dataset and contains a lot of unwanted characters and symbols as shown in the image. 

![Raw data](Raw_data.png)

### Data pre-processing (cleaning) 
Data pre-processing was applied to clean the data from URLs, mentions, hashtags, emojis, excessive repeating characters, and extra spaces. The following image shows the data after cleaning. 

![Clean data](clean_data.png)

##Toknization
GPT2 Byte-Pair Toknizer was used and retrained on our dataset.

##Training
A GPT2 was pre-trained from scratch on our dataset. Due to resource limitations, the model was trained for only 25 epochs. The small size of the data led to overfitting, as shown in the graph. Future work: using a pre-trained model and retraining it on our data might give us way better results. 

![pre-training loss](pre-training_loss.png)














