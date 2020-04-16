# spam-sms-classification-with-ml
![Image](https://appliedmachinelearning.files.wordpress.com/2017/01/spam-filter.png)

### Which one does it catch whole* SPAM SMS?

|__Problem__|__Data__|__Methods__|__Libs__|__Link__|
|-|-|-|-|-|
|`NLP`|Text|`Naive Bayesian`, `SVM`, `Random Forest Classifier`, `Deep Learning - LSTM`, `Word2Vec`|`Sklearn`, `Keras`, `Gensim`, `Pandas`, `Seaborn`|https://github.com/shubhamnag14/spam-sms-classification-with-ml/|

In this project, We applied supervised learning (classification) algorithms and deep learning (LSTM).

We used a public [SMS Spam dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection),which is not purely clean dataset.The data consists of two different columns (features), such as context, and class.The column context is referring to SMS. The column class may take a value that can be either `spam` or `ham` corresponding to related SMS context.

Before applying any supervised learning methods, we applied a bunch of data cleansing operations to get rid of messy and dirty data since it has some broken and messy context.

After obtaining cleaned dataset, we created tokens and lemmas of SMS corpus seperately by using [Spacy](https://spacy.io/), and then, we generated [bag-of-word](https://en.wikipedia.org/wiki/Bag-of-words_model) and [TF-IDF](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) of SMS corpus, respectively. In addition to these data transformations, we also performed [SVD](https://en.wikipedia.org/wiki/Singular-value_decomposition), [SVC](http://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html), [PCA](https://en.wikipedia.org/wiki/Principal_component_analysis) to reduce dimension of dataset.

