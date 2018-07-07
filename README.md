# Project Title:
Prediction of Job Interview Performance by extracting Lexical features.

**Our framework will:-**
* quantify the relative inﬂuences of diﬀerent low level features on the interview performance.
* learns regression models to predict interview ratings and the likelihood of hiring using automatically extracted features.
* predicts several other high-level personality traits such as engagement, friendliness, and excitement.

One of our objectives is to extend the existing automated conversation systems by providing feedback on the overall interview performance and additional high-level personality traits.

# Dependencies:
* Numpy
* Pandas
* Openpyxl
* NLTK
* Matplotlib
* sklearn
* Python3

Use [pip](https://pypi.org/project/pip/) to install any missing dependencies.

```Here we use MIT Dataset. You can find the research paper of MIT here```[Automated Prediction and Analysis of Job Interview Performance](https://ieeexplore.ieee.org/document/7579163/)

# Overview:
**These are step by step process for this project:**
* We extract 21 feature in dataset and some of them are using Linguistic Inquiry Word Count(LIWC)
* We calculate Mutual Information of all features for each personality traits.
* Top seven feature is selected based on Mutual Information for applying Support vector regression(SVR).
* We also apply Random Forest and Lasso to the dataset. And then apply K-Fold cross validation to all algorithm.
* We finally calculate accuracy of each model and comapare them. We also compare Lexical features with the prosody features.
