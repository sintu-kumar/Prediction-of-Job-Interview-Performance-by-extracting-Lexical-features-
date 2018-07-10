# Project Title:
Prediction of Job Interview Performance by extracting Lexical features.

**Our framework will:-**
* quantify the relative inﬂuences of diﬀerent low level features on the interview performance.
* learns regression models to predict interview ratings and the likelihood of hiring using automatically extracted features.
* predicts several other high-level personality traits such as engagement, friendliness, and excitement.

`The objective of the project is to extract the various lexical features responsible for diﬀerent personality traits and predict scores for various personality traits given a text interview.`

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
**Steps followed for this project:**
* First we extract 21 features in dataset and some of them are using Linguistic Inquiry Word Count(LIWC)
* We calculate Mutual Information of all features for each personality traits. `Mutual information (MI) between two random variables is a non-negative value, which measures the dependency between the variables. It is equal to zero if and only if two random variables are independent, and higher values mean higher dependency.`
* Top seven feature is selected based on Mutual Information for applying Support vector regression(SVR). Here we also do feature scaling.
* We also apply Random Forest and Lasso to the dataset. And then apply K-Fold cross validation to all algorithm. `K-Folds cross-validator provides train/test indices to split data in train/test sets. Split dataset into k consecutive folds (without shuffling by default). Each fold is then used once as a validation while the k - 1 remaining folds form the training set.`
* We finally calculate accuracy of each model and comapare them. We also compare Lexical features with the prosody features for different personalty traits.


## Here are some plots of comparison between different algorithm and Lexical features with the prosody features:

`SVR vs Random Forest vs Lasso(respectively) for NoFiller personality traits:`
![svr vs rf vs lasso mean_accuracy](https://user-images.githubusercontent.com/29041062/42410400-bab32d6a-8206-11e8-9f0d-d46f58e02e8d.PNG)



`Lexical features vs prosody features for NoFiller personality traits:`
![rf_com_nf](https://user-images.githubusercontent.com/29041062/42410505-416a1bec-8208-11e8-89e9-d43c2705962e.PNG)

##### `You can contact me at: sintucse@gmail.com`
