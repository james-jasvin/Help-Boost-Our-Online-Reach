# Help Boost Our Online Reach!

This task was done as a Mini-Project for the AI511 - Machine Learning course @ IIIT-B M.Tech CSE

## Problem Statement
Consider yourself to be a consultant for an online advertising agency. The agency spends a considerable amount of time and money to find the best web pages to publish their ads on. They select web pages that will generate prolonged online traffic so that their ads can have a long-lasting reach.

Now, wouldn’t it be great if you could somehow automate this process and save company resources? To facilitate this, the agency has created a dataset of raw html, meta statistics and a binary label for each webpage. The binary label represents whether the webpage was selected for ad placement or not.

The aim of this task is to identify the relevant, high-quality web pages from a pool of user-curated web pages, for the identification of “ad-worthy” web pages. The challenge requires you to build large-scale, end-to-end machine learning models that can classify a website as either “relevant” or “irrelevant”, based on attributes such as alchemy category and its score, meta-information of the web pages and a one-line description of the content of each webpage. This task aims to gently introduce you to the domain of NLP, as you would be required to convert the string attributes of the dataset to some form of numerical data, and then construct your ML models on this numerical data.

Can this fast-paced ad agency bank on you to deliver on this project?

[Note: Evaluation is done using ROC score of probabilities and not absolute predictions].

## Key Elements
- Applied basic preprocessing techniques to do EDA on the data.
- Used URL data to engineer websiteName feature.
- Applied NLP preprocessing techniques on the websiteDescription data.
- Preprocessed text data was given to the TF-IDF Vectorizer to get feature vectors with vocabulary size of 10000 words.
- Standard sklearn classification models like Logistic Regression, Random Forest, SVM, etc. were applied on this data.
- Used Chi-Squared Test to reduce vocabulary size to 305 words and still retain same score.
- Word2Vec was applied using two approaches (sentences & trigrams) to obtain word vectors which were then averaged to get feature vectors.
- Standard sklearn classification models + various architectures for the MLP Classifier were tried on this data.
- The best results were obtained with Trigrams Word2Vec with averaging approach + 4-Layer MLP architecture.

##
Check Final Report.pdf for a full overview of what was done in this project.
