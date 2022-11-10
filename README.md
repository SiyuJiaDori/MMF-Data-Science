# MMF-Data-Science
MMF Data Science final project

Siyu Jia

Abstract
This report examined and predicted the prices of diamonds using the random forest model. The prediction was based on various variables including diamonds’ weight, color, cut quality, clarity, etc. The final target is to get a predicted price of the diamonds and beat the benchmark.

Introduction
The Random Forest is built up of a large number of individual decision trees that work as an ensemble, and each tree in the random forest will have its class prediction and choose the one with the most votes as our final prediction. In random forest, ntree shows how many trees the user chooses to grow and mtry represents the number of variables we choose at each split. The project also uses prediction code to train and apply the output. Eventually, the model uses the test set to check the goal and returns the output CSV.

Feature Engineering Method
To gain an overview of the data frame, I used the skim method from the skim package to check the data type and see if there have missing data. Based on the information it provided, there are no missing data in the data set, but three character variables which are cut, color, and clarity in the data set. In this case, I used the factor method to change them into factor variables because characters are not supported in the machine learning algorithm. Additionally, to better build the relation between price and these ordinal categorical variables. I used the number to represent the level of variables from lowest to highest and return to the data set to make a future analysis.

Model Setup
In the model setup, I import the randomForest package to build the model. For more details, due to the computer capacity, I set up ten trees in the random forest model. Moreover, in the skim method used at the beginning, I got a histogram return which can imply the impact of every variable. Based on the histogram, I kept all the variables to use in the model because they seemingly all have some impact on the price.

Conclusion
The final submission at Kaggle is 568.75295 which beats the benchmark.


