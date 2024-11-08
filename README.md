# Financial Market Sentiment Prediction

## Project Description
This project aims to develop models to predict financial market sentiment from texts. We explore both Machine Learning-based approaches and language models (LLMs) to identify the best performers for the sentiment classification task.

Here you can explore the [notebook](https://github.com/erickmaiia/ml-financial-sentiment-analysis/blob/main/notebook.ipynb) with this experiment in more detail

We chose to follow a sequence of steps in the development of this experiment:

### 1. Preprocessing
We perform preprocessing of the textual data, including text cleaning, stopword removal, and word transformation for a more appropriate representation. These steps are essential to ensure that the models can process the text effectively.

### 2. Exploratory Data Analysis (EDA)
In exploratory data analysis, we investigated the characteristics of the data and visualized the class distribution, average text size, and other aspects relevant to building machine learning models. This helped us better understand the nature of the data and identify possible adjustments in preprocessing.

### 3. Machine Learning-Based Approach
Initially, we tested a variety of Machine Learning algorithms for sentiment classification. The algorithms used include:

- Random Forest
- Gradient Boosting
- AdaBoost
- LightGBM
- XGBoost
- Decision Tree
- Support Vector Machine
- Naive Bayes
- Multilayer Perceptron

These approaches proved to be unsatisfactory in terms of accuracy, leading us to explore more sophisticated alternatives.

### 4. Transformers as an Alternative
Given the limited results with Machine Learning models, we chose to use a robust language model (LLM), **RoBERTa**, which was pre-trained on large volumes of data. Although transformers require greater processing capacity, RoBERTa significantly outperformed Machine Learning models, achieving an accuracy of **86.32%** after only 5 epochs of fine-tuning.

**Note:** We did not directly use heavier transformer models in projects, as their high computational demand would make practical application difficult in the context of the project.

### 5. Conclusion
We conclude that, although Machine Learning models offer fast solutions, the performance in terms of accuracy for sentiment classification in the financial market is significantly improved with the use of pre-trained language models, such as RoBERTa. These models are more effective in capturing nuances of sentiment, making them more suitable for complex text classification tasks.

This project is a solid foundation for developing financial market sentiment analysis models, with important insights into the use of LLMs and traditional machine learning approaches for text analysis.
