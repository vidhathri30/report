

## Task1

The data is imported as a pandas dataframe, then we add the house prices to it. This will allow us to manipulate this data mathematically by using inbuilt methods in pandas which is called data cleaning.

We will start with importing basic modules such as numpy, pandas and matplotlib. We put the data into a data frame which behaves like an 2D array in C, using Pandas. With data frames we can manipulate the data mathematically by using inbuilt methods in pandas which is called data cleaning.

We will use a set of data that helps us understand the relationship between variables. We import numpy to convert the data from Pandas into a 2D array. Then we can manipulate the data mathematically by adding columns and slicing it in different ways with pd.DataFrame().

Linear Regression is a supervised learning algorithm, which means that it works on a set of labeled examples. Before we look at how to use linear regression in Python, let's first learn about the concepts we need to understand before using the appropriate methods,

The steps involved in implementing the model are as follows:

1.  Initially the libraries are imported

    ![task11](https://user-images.githubusercontent.com/116189666/227711961-217a5166-d013-488f-8851-2c75876959ed.jpg)


2.  The Boston housing price data is loaded from the datasets. The target contains the prices of the houses feature_names contain the names of all the features in the dataset (except target variables). Before moving on to the next step, the data is checked for any missing values i.e the null values. There are no missing values in the dataset

   ![task12](https://user-images.githubusercontent.com/116189666/227711972-3c1c0e6c-ee63-4338-ba80-043dd68cd4ca.jpg)


3.  The data splitted as training data and testing data The size value 0.2 indicates that 80% of the samples are used to train the model and the remaining 20% to evaluate or test the model. For this purpose, we use we utilize the scikit learn library's train_test_split() function as shown
![task13](https://user-images.githubusercontent.com/116189666/227711978-136a6c3c-f82f-4856-9d54-01e98c93af24.jpg)


4.  Scikit learn's LinearRegression() is used to train our model on both the training and test sets

![task14](https://user-images.githubusercontent.com/116189666/227711986-595c63b1-dc57-4316-a648-07b9b9fededf.jpg)

5.  This step is to determine whether the model is overfitting or not. Overfitted models perform well on test datasets but do not predict well on real-world datasets The root mean squared error(rms) and R2 score is used to assess the overfitting. The R2 score is of both training and testing data are almost equal to one. Hence the model is not overfitting
![task15](https://user-images.githubusercontent.com/116189666/227711993-ecf25a6b-ee17-4c32-bbf3-46c24b171cea.jpg)


6.Finally the actual prices vs predicted prices are visualized using scatter plot

![task16](https://user-images.githubusercontent.com/116189666/227712000-5da5a1a3-4d4e-444e-b001-bfa9e8dabf09.jpg)
