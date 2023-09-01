# Sentiment Analysis on crypto related comments using DistilBERT

## Overview
This project involves a sentiment analysis (also known as opinion mining) on comments from the crypto community. The analysis utilizes Transformers models, specifically BERT and DistilBERT, as well as traditional Feed Forward Networks (FFN) and Convolutional Neural Networks (CNN). The primary objective is to assess the effectiveness of fine-tuning these models for the crypto domain, which contains specialized terms and idioms commonly used by its users. The project also compares the performance of FFN, CNN, BERT, and DistilBERT models.

The fine-tuning process employs pre-trained Transformers models, BERT and DistilBERT, available through the [HuggingFace](https://huggingface.co/) Python library. A labeled dataset from [Social-Grep](https://socialgrep.com/), consisting of comments from various crypto-related subreddits in August 2021, is used for training, validation, and testing the DistilBERT model. Additionally, an unlabeled dataset exclusively from the "r/cryptocurrency" subreddit is used for experiments. This dataset is collected using the PushShift API for Reddit and the pmaw wrapper.

The project explores the performances of the models and the effects of fine-tuning as well as the correlation between Bitcoin's price (the most popular cryptocurrency) and the sentiment of the crypto community. The findings reveal that during market crashes in November 2021, the sentiment score significantly declined compared to previous days, indicating a strong relationship between cryptocurrency price movements and community sentiment. 
This project was made for the Human Language Technologies exam (A.Y. 2021-2022) @ University of Pisa.

## Programming Language/Framework
Python, PyTorch and Tensorflow, Jupyter

## Results
We experimented with different configurations of the models and amount of data, in this way we obtained a final DistilBERT model which achieves an accuracy of <b>95%</b> on the test set. 
We observed that in the experiments the DistilBERT version took half of the time and it also had a similar performance with respect to the corresponding BERT model. 
Finally we showed a practical example of how to analyze the movements of the crypto market in comparison to the sentiment showing that the approach is well-founded.

The figure below shows the correlation between Bitcoin price (candlesticks) and the sentiment score.
![image](https://github.com/luca-santarella/sentiment-analysis-crypto/assets/67547343/34ccfb4f-10b7-4a10-a92f-2c3dfb695783)



