# fastText-Real-or-Not-NLP-with-Disaster-Tweets

 Experimenting with fasttext on tweets.
 Predict which Tweets are about real disasters and which ones are not
 Trains on CPU , compatible with Linux cmd line for auto-tune-validation.
 


## Hyperparameters of supervised model:
- **label_prefix :** The librarry needs a prefix to be added to classification labels
- **lr:** The learning rate...works well with default (0.1) lr.
- **neg :** Number of negative samples 2<neg<6
- **epoch :** 5,10,15 
- **dim :** 128,256 perform very well.
- **loss:** softmax takes a bit longer ,hs hierarchial softmax is good too, ns not good score.
- **word_ngrams:** 2=bigrams ,3=trigrams ,in this case limit it to 2 as per original paper + score_performance
- **ws:** Size of context window ,here avg sentence length is not too large ,therefore we chose 3 based on experiments.
- **bucket:** Hash length
-**


 # Note:
 Above task can be completed using TFIDF,SVM,BERT,GloVE,LSTM,etc but training time is really high.
 ## Essential Reads:
- [PythonDocs](https://fasttext.cc/docs/en/python-module.html)
- [Enriching Word Vectors with Subword Information](https://arxiv.org/abs/1607.04606)
- [Bag of Tricks for Efficient Text Classification](https://arxiv.org/abs/1607.01759)
- [Open-sourcing hyperparameter autotuning for fastText](https://ai.facebook.com/blog/fasttext-blog-post-open-source-in-brief/)
- [English word vectors](https://fasttext.cc/docs/en/english-vectors.html)
