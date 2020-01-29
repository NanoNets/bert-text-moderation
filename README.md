## Toxic Comments Classification using BERT and CNNs

The companion blog post on [text moderation](https://nanonets.com/blog/text-moderation) can be found here. 

The dataset used is from the kaggle Toxic Comments Challenge and can be downloaded from [here](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/overview).

### Overview

The labels in the dataset are 
```labels = ['toxic', 'severe_toxic', 'obscene', 'threat', 'insult', 'identity_hate']```

The CNN architecture used is an implementation of [this](paper) as found [here](https://towardsdatascience.com/identifying-hate-speech-with-bert-and-cnn-b7aa2cddd60d). We use the Hugging Face Transformers library to get word embeddings for each of our comments. We transfer these weights and train our CNN model based on our classification targets. 

