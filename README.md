# Word Embeddings for the Armenian Language: Intrinsic and Extrinsic Evaluation

### Pretrained Embeddings

We release pre-trained word embeddings:
- 200-dimensional GloVe vectors ([.text](https://at.ispras.ru/owncloud/index.php/s/pUUiS1l1jGKNax3));
- 300-dimensional CBOW ([.text](https://at.ispras.ru/owncloud/index.php/s/1OwoRvaxazM9Yy2)) and SkipGram ([.text](https://at.ispras.ru/owncloud/index.php/s/oQnHLnUo10zA3dJ)) vectors;
- 200-dimensional fastText vectors ([.text](https://at.ispras.ru/owncloud/index.php/s/eDOUye5Ka4uC3lB), [.bin](https://at.ispras.ru/owncloud/index.php/s/CxnJH6QQioCYpLc)), trained using SkipGram  architecture, with char n-grams up to length 3.

The training data for these models was collected from various sources:

a. Wikipedia;\
b. fiction  texts  taken  from  the  open  part  of  the EANC corpus;\
c. HC Corpora containing blogs and news articles collected by Hans Christensen from public sources in 2011;\
d. digitized and reviewed part of Armenian soviet encyclopedia (as of February 2018) taken from Wikisource;\
e. texts from news websites on the following topics: economics, events, art, sports, law, politics, blogs and interviews.

The texts were preprocessed by lowercasing all tokens and removing punctuation, digits. The final dataset contained 90.5  million tokens.


### Word Analogy Task

In addition, we publish an adaptation of the word analogy task ([Mikolov et al., 2013a](https://arxiv.org/pdf/1301.3781.pdf)) for the Armenian language to serve as benchmark for intrinsic evaluation of vectors. The task contains 5 semantic and 8 syntactic sections, with 15646 analogy questions in total.

### News Texts Dataset

For extrinsic evalution of vectors in a classification task, we release a dataset of over 12000 news articles from [iLur.am](http://www.ilur.am/), categorized into 7 classes: sport, politics, weather, economy, accidents, art, society. The articles are split into train (2242k tokens) and test sets (425k tokens).

For more details, refer to the [paper]().
