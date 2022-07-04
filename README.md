# Machine Learning Trading Bot

In this Challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.

## Instructions:

Use the starter code file to complete the steps that the instructions outline. The steps for this Challenge are divided into the following sections:

- Establish a Baseline Performance

- Tune the Baseline Trading Algorithm

- Evaluate a New Machine Learning Classifier

- Create an Evaluation Report


2. Baseline 


- Import the OHLCV dataset into a Pandas DataFrame.

- Generate trading signals using short- and long-window SMA values.

- Split the data into training and testing datasets.

- Use the SVC classifier model from SKLearn's support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Review the predictions.

- Review the classification report associated with the SVC model predictions.

- Create a predictions DataFrame that contains columns for “Predicted” values, “Actual Returns”, and “Strategy Returns”.

- Create a cumulative return plot that shows the actual returns vs. the strategy returns. Save a PNG image of this plot. This will serve as a baseline against which to compare the effects of tuning the trading algorithm.

### Baseline conlcusion 
The baseline model did slightly better than flipping a coin, with accuracy of 65% and F1 score at 77%. 

## Tune the Baseline Trading Algorithm
In this section, you’ll tune, or adjust, the model’s input features to find the parameters that result in the best trading outcomes. (You’ll choose the best by comparing the cumulative products of the strategy returns.) To do so, complete the following steps:

- different from original slice of data, we have choosen a broader range of dates, which is for 4 years

Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. 
- adjusted the SMA to 60 days and 120 days

Import a new classifier, such as AdaBoost, DecisionTreeClassifier, or LogisticRegression. (For the full list of classifiers, refer to the Supervised learning page in the scikit-learn documentation.)
- Adaboost as new model 

Using the original training data as the baseline model, fit another model with the new classifier.

### Summary
In the updated model under the same baseline, the model did not end have a better prediciton, only with 58% accuracy and F1 score of 72%, mainly becasue in this updated model, we over trained the dataset

