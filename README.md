https://www.kaggle.com/rmisra/news-headlines-dataset-for-sarcasm-detection?select=Sarcasm_Headlines_Dataset_v2.json

# News-Headlines-Dataset-For-Sarcasm-Detection

Past studies in Sarcasm Detection mostly make use of Twitter datasets collected using hashtag based supervision but such datasets are noisy in terms of labels and language. Furthermore, many tweets are replies to other tweets and detecting sarcasm in these requires the availability of contextual tweets.

To overcome the limitations related to noise in Twitter datasets, this **Headlines dataset for Sarcasm Detection** is collected from two news website. [*TheOnion*](https://www.theonion.com/) aims at producing sarcastic versions of current events and we collected all the headlines from News in Brief and News in Photos categories (which are sarcastic). We collect real (and non-sarcastic) news headlines from [*HuffPost*](https://www.huffingtonpost.com/).

This new dataset has following advantages over the existing Twitter datasets:
* Since news headlines are written by professionals in a formal manner, there are no spelling mistakes and informal usage. This reduces the sparsity and also increases the chance of finding pre-trained embeddings.
* Furthermore, since the sole purpose of *TheOnion* is to publish sarcastic news, we get high-quality labels with much less noise as compared to Twitter datasets.
* Unlike tweets which are replies to other tweets, the news headlines we obtained are self-contained. This would help us in teasing apart the real sarcastic elements.

## Data
Each record consists of three attributes:

* ```is_sarcastic```: 1 if the record is sarcastic otherwise 0

* ```headline```: the headline of the news article

* ```article_link```: link to the original news article. Useful in collecting supplementary data

## Overview
This data set is a collection of headlines from 2 sources - The Onion and The Huffington Post - the former being an exclusively satirical publication and the latter being a mixture of both satire and serious pieces. Each headline contains headlines as strings of between 10 and 15 words of which there are just shy of 27000 data points. The aim is to classify each of these headlines as either sarcastic or serious.
