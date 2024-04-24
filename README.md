In this project, we are trying to analyze a used car dataset from Kaggle. We are gonna to follow the CRISP_DM framework to do the data analysis. The analyzing notebook is located at

1. Business Understanding
   By analyzing the data, try to find the parameters which have realtively large permutation importance and build the relationship between the paras and price.

 2.  Data Understanding
    The general data info is shown below. This data has 42688 * 17. Most of the Columns are 'object'.
    ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/a4dccced-6573-4c52-a6c2-cb3b8d4f9502)

     The numerical data desribe() is show below.
     ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/9c50753d-cc9e-4844-96ce-a80fb9a418a5)

     check the columns with null value and plot
     ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/4530fc6d-8318-4d29-a60e-ef2992afc9af)

     Based on the plot, we see that column 'Size', most of the values are null. And considering 'id', 'VIN' are the identify infomation of a car, which is not contributing to the final price. We remove these three columns from the dataset.
     In addition, we consider the location information will affect the car prices evenly for all the model and types. We only focus on the data from california.
     This is the example of the final analyzing data.
     ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/06cec538-81ab-46f5-b60a-eb98baae58ff)
     ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/01635cbe-a003-44ad-b15d-9f580217a355)


     For cross validation, we split the data into two set. X_train(70%), X_test(30%)
     ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/4529f859-b910-4617-aa80-a5197040f973)




     




