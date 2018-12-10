# Titanic_Kaggle
the goal is to predict the survival or the death of a given passenger based on 12 feature such as sex, age ,etc...
what will you read in this tutorial?

-----------------------------------------

1 Define Problem

2 Installation

3 Import Machine learning libraries

4 EDA

5 Feature Engineering

6 Modeing

7 Feature Selection

8 Conclusion

-----------------------------------------

# 1 Define Problem
this is a binary classification to detect survived people. we have two datasets, train, and test.
when we build our model we should predict for the new passenger that he or she were been survived or dead.
# 1-1 introduction

RMS Titanic was a British passenger liner that sank in the North Atlantic Ocean in the early hours of 15 April 1912, after colliding with an iceberg during its maiden voyage from Southampton to New York City. There were an estimated 2,224 passengers and crew aboard, and more than 1,500 died, making it one of the deadliest commercial peacetime maritime disasters in modern history. RMS Titanic was the largest ship afloat at the time it entered service and was the second of three Olympic-class ocean liners operated by the White Star Line. It was built by the Harland and Wolff shipyard in Belfast. Thomas Andrews, her architect, died in the disaster.

# 1-2 dataset

Titanic dataset is an open dataset where you can reach from many different repositories and GitHub accounts. However, downloading from Kaggle will be definitely the best choice as the other sources may have slightly different versions and may not offer separate train and test files. So, please visit this link to download the datasets (Train.csv and Test.csv) to get started.

-----------------------------------------
# 2- installation

A very easy way to install these packages is to download and install the Conda distribution that encapsulates them all. This distribution is available on all platforms (Windows, Linux and Mac OSX).

-----------------------------------------
# 3- Import

Throughout this jupyter notebook, I will be using Python at each level of the pipeline.

The main libraries involved in this tutorial are:

Pandas for data manipulation and ingestion
Matplotlib and seaborn for data visualization
Numpy for multidimensional array computing
sklearn for machine learning and predictive modeling

-----------------------------------------
# 4 - Exploratory data analysis

As in different data projects, we'll first start diving into the data and build up our first intuitions.

In this section, we'll be doing four things.

Data extraction : we'll load the dataset and have a first look at it.
Cleaning : we'll fill in missing values.
Plotting : we'll create some interesting charts that'll (hopefully) spot correlations and hidden insights out of the data.
Assumptions : we'll formulate hypotheses from the charts.


-----------------------------------------
# 5 - feature engineering
In the previous part, we flirted with the data and spotted some interesting correlations.

In this part, we'll see how to process and transform these variables in such a way the data becomes manageable by a machine learning algorithm.

We'll also create, or "engineer" additional features that will be useful in building the model.

We'll see along the way how to process text variables like the passenger names and integrate this information in our model.

We will break our code in separate functions for more clarity.

But first, let's define a print function that asserts whether or not a feature has been processed.
# 5-1 Loading The Data
One trick when starting a machine learning problem is to append the training set to the test set together.

We'll engineer new features using the train set to prevent information leakage. Then we'll add these variables to the test set.

Let's load the train and test sets and append them together.
# 5-2 Extracting the passenger titles
When looking at the passenger names one could wonder how to process them to extract a useful information.

If you look closely at these first examples:

Braund, Mr. Owen Harris Heikkinen, Miss. Laina Oliva y Ocana, Dona. Fermina Peter, Master. Michael J You will notice that each name has a title in it ! This can be a simple Miss. or Mrs. but it can be sometimes something more sophisticated like Master, Sir or Dona. In that case, we might introduce an additional information about the social status by simply parsing the name and extracting the title and converting to a binary variable.

Let's see how we'll do that in the function below.

Let's first see what the different titles are in the train set

-----------------------------------------
# 6- Modeling

In this part, we use our knowledge of the passengers based on the features we created and then build a statistical model. You can think of this model as a box that crunches the information of any new passenger and decides whether or not he survives.

There is a wide variety of models to use, from logistic regression to decision trees and more sophisticated ones such as random forests and gradient boosted trees.

We'll be using Random Forests. Random Froests has proven a great efficiency in Kaggle competitions.

For more details about why ensemble methods perform well, you can refer to these posts:

http://mlwave.com/kaggle-ensembling-guide/

http://www.overkillanalytics.net/more-is-always-better-the-power-of-simple-ensembles/

Back to our problem, we now have to:

Break the combined dataset in train set and test set.

Use the train set to build a predictive model.

Evaluate the model using the train set.

Test the model using the test set and generate and output file for the submission.

Keep in mind that we'll have to reiterate on 2. and 3. until an acceptable evaluation score is achieved.


Let's start by importing the useful libraries.

-----------------------------------------
# 7 - Conclusion
In this article, we explored an interesting dataset brought to us by Kaggle.

We went through the basic bricks of a data science pipeline:

Data exploration and visualization: an initial step to formulate hypotheses
Data cleaning
Feature engineering
Feature selection
Hyperparameters tuning
Submission
Blending

# Help

I hope you have enjoyed reading my python notebook.

If you have any problem and question to run notebook please open an issue here in github.

for most of the my notebook you need **dataset** as input.

To use the **correct data**, please **download** the dat set from  the **Kaggle** site and put it in your notebook folder.

**Mj Bhamnai**

mohamadjavad.bahmani@gmail.com

 **Have Fun!**
 
> ###### 1. Follow me On [GitHub](https://github.com/mjbahmani/)
 
> ###### 2. Follow me On [Kaggle](https://www.kaggle.com/mjbahmani)
