# fastText-Real-or-Not-NLP-with-Disaster-Tweets

 Predict which Tweets are about real disasters and which ones are not
 
-----
## Hyperparameters:
- **label_prefix :** The librarrty assumes a prefix to be added to classification labels
- **lr:** The learning rate...
- **neg :** Number of negative samples 2<neg<6
- **epoch :** 5,10,15 works well incase of default (0.1) lr.
- **dim :** 128,256 perform very well.
- **loss:** softmax takes a bit longer ,hs hierarchial softmax is good too, ns not good score.
- **word_ngrams:** 2=bigrams ,3=trigrams ,in this case limit it to 2 as per original paper + score_performance
- **ws:** Size of context window ,here avg sentence length is not too large ,therefore we chose 3 based on experiments.
- **bucket:** Hash length
