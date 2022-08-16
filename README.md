# Sentiment-Analysis-Amazon-Fine-Food-Reviews

DATASET LINK : https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews

## About Dataset
### Context
  * This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

### Contents
  * Reviews.csv: Pulled from the corresponding SQLite table named Reviews in database.sqlite

## About Project
In this project, I will be using Three different Techniques
  * VADER (Valence Aware Dictionary and sentiment Reasoner) - Bag of words approach
  * Roberta Pretrained Model from HuggingFace
  * Huggingface Pipeline
  
**Objective : To generate the sentiments from the text in the dataset and comparing the above three different techinques**

Loaded the dataset using pandas library
NLTK package is used to tokenize the text for further analysis
NLTK is a popular Python framework for dealing with data of human language. It includes a set of text processing libraries for classification and semantic reasoning, as well as wrappers for industrial-strength NLP libraries and an active discussion forum. NLTK is ideal for linguists, engineers, students, and industry users. Nltk is very useful in a python programming language. Nltk in python we can learn new thing, nltk is very useful to learn new technology.

Performed basic NLTK and EDA

Applied Vader techinque to generate the sentiments.
* VADER (Valence Aware Dictionary and sEntiment Reasoner) is a pre-trained model that uses rule-based values tuned to sentiments from social media. It evaluates the text of a message and gives you an assessment of not just positive and negative, but the intensity of that emotion as well.

Applied Roberta Pretrained Model from HuggingFace
* RoBERTa is a transformers model pretrained on a large corpus of English data in a self-supervised fashion. This means it was pretrained on the raw texts only, with no humans labelling them in any way (which is why it can use lots of publicly available data) with an automatic process to generate inputs and labels from those texts.

Compared both the model using pairplot

**Conclusion:**
Both the model provided the correct output. But in reviews there were text which were sarcastic too for those kind of statements roberta was more effective than vader
