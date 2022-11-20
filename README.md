Module 14
================================

![image](https://user-images.githubusercontent.com/104800728/202930995-4076dcfc-7ae8-443c-98ba-7376dbb596ba.png)

Background
-----------------------

For this Challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.

What You're Creating
-----------------------

You’ll combine your new algorithmic trading skills with your existing skills in financial Python programming and machine learning to create an algorithmic trading bot that learns and adapts to new data and evolving markets.

In a Jupyter notebook, you’ll do the following:

- Implement an algorithmic trading strategy that uses machine learning to automate the trade decisions.

- Adjust the input parameters to optimize the trading algorithm.

- Train a new machine learning model and compare its performance to that of a baseline model.

As part of the README.md file in your GitHub repository, you’ll also create a report that compares the performance of the machine learning models based on the trading predictions that each makes and the resulting cumulative strategy returns.

Files
-----------------------

Download the following files to help you get started: 
- Module 14 Challenge files

Instructions
-----------------------

The steps for this Challenge are divided into the following sections:

- Establish a Baseline Performance

- Tune the Baseline Trading Algorithm

- Evaluate a New Machine Learning Classifier

- Create an Evaluation Report

Establish a Baseline Performance
-----------------------

In this section, you’ll run the provided starter code to establish a baseline performance for the trading algorithm. To do so, complete the following steps.

NOTE The provided CSV file contains open, high, low, close, and volume (OHLCV) data for a Morgan Stanley Capital International (MSCI)–based emerging markets exchange-traded fund (ETF) that iShares (Links to an external site.) issued. Investments in emerging markets make up an important aspect of a well-diversified investment portfolio. That’s because the included equities have potentially higher long-term returns, even though they carry more risk.

1. Open the provided Jupyter notebook, restart the kernel, and then run the cells that correspond with the following steps:
- Import the OHLCV dataset into a Pandas DataFrame.

- Generate trading signals by using short- and long-window SMA values.

- Split the data into training and testing datasets.

2. Use the SVC classifier model from the SKLearn support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Review the predictions.

3. Review the classification report that’s associated with the SVC model predictions.

4. Create a predictions DataFrame that contains “Predicted”, “Actual Returns”, and “Strategy Returns” columns.

5. Create a cumulative return plot that shows the actual returns vs. the strategy returns. Save a PNG image of this plot. This will serve as a baseline against which to compare the effects of tuning the trading algorithm.

6. Write your conclusions about the performance of the baseline trading algorithm in the README.md file that’s associated with your GitHub repository. Support your findings by using the PNG image that you saved in the previous step.

Tune the Baseline Trading Algorithm
-----------------------

In this section, you’ll tune, or adjust, the model’s input features to find the parameters that result in the best trading outcomes. (You’ll choose the best by comparing the cumulative products of the strategy returns.) To do so, complete the following steps:

1. Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file. Answer the following question: What impact resulted from increasing or decreasing the training window?
HINT To adjust the size of the training dataset, you can use a different DateOffset value—for example, six months. Be aware that changing the size of the training dataset also affects the size of the testing dataset.

2. Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your README.md file. Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?

3. Choose the set of parameters that best improved the trading algorithm returns. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file.

Evaluate a New Machine Learning Classifier
---------------------------------------------

In this section, you’ll use the original parameters that the starter code provided. But, you’ll apply them to the performance of a second machine learning model. To do so, complete the following steps:

1. Import a new classifier, such as AdaBoost, DecisionTreeClassifier, or LogisticRegression. (For the full list of classifiers, refer to the Supervised learning page (Links to an external site.) in the scikit-learn documentation.)

2. Using the original training data as the baseline model, fit another model with the new classifier.

3. Backtest the new model to evaluate its performance. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns for this updated trading algorithm, and write your conclusions in your README.md file. Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?

Create an Evaluation Report
---------------------------------------------

In the previous sections, you updated your README.md file with your conclusions. To finish this section, add a summary evaluation report at the end of the README.md file. For this report, express your final conclusions and analysis. Support your findings by using the PNG images that you created.

Requirements
=========================

Establish a Baseline Performance (25 points)
---------------------------------------------

To receive all points, you must:

- Use the SVC classifier model from SKLearn's support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. (6 points)

- Review the classification report associated with the SVC model predictions. (5 points)

- Create a predictions DataFrame that contains columns for “Predicted” values, “Actual Returns”, and “Strategy Returns”. (6 points)

- Create a cumulative return plot that shows the actual returns vs. the strategy returns. (6 points)

- Save a PNG image of the cumulative return plot. This will serve as a baseline against which to compare the effects of tuning the trading algorithm. (1 point)

- Write your conclusions about the performance of the baseline trading algorithm in the README.md file that’s associated with your GitHub repository. Support your findings by using the PNG image that you saved in the previous step. (1 point)

Tune the Baseline Trading Algorithm (10 points)
---------------------------------------------

To receive all points, you must:

- Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters To show this work, record the results in your README.md file. (4 points)

- Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters. To show this work, record the results in your README.md file. (4 points)

- Choose the set of parameters that best improved the trading algorithm returns. To show this work, save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file. (2 points)

Evaluate A New Machine Learning Classifier (25 points)
---------------------------------------------

To receive all points, you must:

- Import a new classifier, such as AdaBoost, DecisionTreeClassifier, or LogisticRegression. (5 points)

- Using the original training data as the baseline model, fit another model with the new classifier. (10 points)

- Backtest the new model to evaluate its performance. (10 points)

Create an Evaluation Report (10 points)
---------------------------------------------

To receive all points, you must:

- Add a summary evaluation report at the end of the README.md file. For this report, express your final conclusions and analysis. Support your findings by using the PNG images that you created. (10 points)

Coding Conventions and Formatting (10 points)
---------------------------------------------

To receive all points, you must
Place imports at the top of the file, just after any module comments and docstrings, and before module globals and constants. (3 points)

Name functions and variables with lowercase characters, with words separated by underscores. (2 points)

Follow DRY (Don't Repeat Yourself) principles, creating maintainable and reusable code. (3 points)

Use concise logic and creative engineering where possible. (2 points)

Deployment and Submission (10 points)
-----------------------

To receive all points, you must:
- Submit a link to a GitHub repository that’s cloned to your local machine and that contains your files. (5 points)

- Include appropriate commit messages for your files. (5 points)

Code Comments (10 points)
-----------------------

To receive all points, your code must:

- Be well commented with concise, relevant notes that other developers can understand. (10 points)

Submission
-----------------------
- To submit your Challenge assignment, click Submit, and then provide the URL of your GitHub repository for grading.

NOTE You are allowed to miss up to two Challenge assignments and still earn your certificate. If you complete all Challenge assignments, your lowest two grades will be dropped. If you wish to skip this assignment, click Next, and move on to the next module.

Comments are disabled for graded submissions in Bootcamp Spot. If you have questions about your feedback, please notify your instructional staff or your Student Success Manager. If you would like to resubmit your work for an additional review, you can use the Resubmit Assignment button to upload new links. You may resubmit up to three times for a total of four submissions.

Summary
-----------------------

What impact resulted from increasing or decreasing the training window? Decreasing the long window to 50 created a tighter match between the 'Strategy' and 'Actual' returns, thus increasing the accuracy when using a Logistic Regression model

What impact resulted from increasing or decreasing either or both of the SMA windows? By doubling the original short_window = 4, long_window = 100 to short_window = 8, long_window = 200, the strategy predictions deviate greater and the accuracy decreases if using a Logistic Regression model
