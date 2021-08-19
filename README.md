# nlp-abstract-classification
Classification of PubMed abstracts using a NLP-based approach

As the amount of publicly available literature continues to rapidly grow, it is increasingly important for researchers to have improved tools to effectively skim through text. Browsing through literature can be a time-consuming and inefficient task, thus the development of accurate text classification algorithms could prove incredibly useful. By developing and tuning a number of different classification models we aim to identify optimal machine learning algorithms for automatic detection of attributes of a scientific abstract, to assist automatic information extraction from unstructured literature.

Using the PubMed 20k RCT dataset, we evaluate the performance of tf-idf and Doc2Vec feature extraction in combination with naive bayes, logistic regression, support vector machines, and random forest classifiers. Our findings show that although Doc2Vec boosts performances during training, this improvement does not translate to a test set. Moreover, we report that the limiting factor for these models is separating semantically similar sentences such as the "background" and "objective" parts of abstracts.

Best performances were found with a combination of tf-idf vectorization and L2-regularized logistic regression which yielded a macro-F1 score of 69.5% on the test set. In future research, novel feature extraction methods have the potential to increase the performance of text classification even further.
