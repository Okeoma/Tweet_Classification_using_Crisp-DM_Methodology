# Tweet Classification using Crisp-DM Methodology
Development of a Natural Language Processing (NLP) pipeline that demonstrates scientific techniques, critical evaluation skills, and utilizes industrial standard tooling. The objective is to solve the task of multi-class classification of tweets from a popular social media platform, using the CRISP-DM methodology

## METHODOLOGY
The methodology applied in this research project aimed to develop a Natural Language Processing (NLP) pipeline for multi-class classification of tweets. The CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology was followed, encompassing several stages to achieve the research objectives. The methodology involved data understanding, data exploration, data preparation, modeling, and final metrics evaluation.

The initial stage of business understanding involved defining research project goals. This focused on achieving the most accurate result for multi-class classification of tweets. The task was to develop a pipeline that classifies tweets into six categories: Arts & Culture, Business & Entrepreneurs, Pop Culture, Daily Life, Sports & Gaming, and Science & Technology.

The data understanding phase utilized a JSON dataset consisting of 6,443 entries, representing Twitter tweets. These tweets were collected between 2019 and 2021 and manually labeled using Amazon's Mechanical Turk. The dataset was loaded using the Pandas library, and data quality was assessed to ensure no missing values.

During the data exploration stage, data visualization techniques were applied to gain insights and identify patterns within the dataset. The Matplotlib library was used to create bar and pie charts, which provided a visual representation of the dataset's distribution. It was observed that the classes in the label column were imbalanced, with 'Pop Culture' and 'Sports & Gaming' having the highest number of labeled tweets. To address this, stratification techniques were implemented during the dataset splitting process to ensure a uniform distribution of the outcome variable in all subsets.

In the data preparation phase, data processing techniques were applied to clean and preprocess the dataset. Several functions were defined to remove improper words, devanagari language script, punctuation, tokenize the text, and remove stopwords. These cleaning functions were tested on the dataset and found effective. Three data processing functions were defined, each applying the same cleaning steps but with different pre-processing methods: no pre-processor, stemming, and lemmatization. The effectiveness of these functions was evaluated by applying the Textprocessing() function (no pre-processor) to the dataset. Additionally, a word cloud was generated using the WordCloud library to visually represent a portion of the cleaned dataset. See Figure 2 for the presentation of the processed dataset in JSON format and the word cloud.

The modeling phase involved applying various machine learning models to the prepared data. Initially, Naive Bayes was employed, followed by other models such as Multi-Layer Perceptron (MLP) and Gradient Boosting classifiers. A K-Fold method was utilized to split the dataset into train and test subsets, ensuring uniform class distribution. The GridSearchCV pipeline from sklearn.model_selection was integrated to evaluate model performance with different hyperparameters. Multiple versions of the classifier were trained in parallel, and the configuration producing the most impressive results on evaluation metrics was selected.

In the final metrics evaluation stage, the selected model's performance was assessed against the business objectives. The dataset was split into training and testing sets. Performance metrics such as Accuracy score, Precision score, Recall score, and F1 score were calculated on the test set. For visual and tabular representation of the evaluation results, a confusion matrix and Classification report were used.


:arrow_forward: &nbsp; **View Live Application Demonstration [here](https://youtu.be/X0L1zX-lW5Y)**

