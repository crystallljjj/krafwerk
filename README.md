In this project, we are trying to analyze a used car dataset from Kaggle. We are gonna to follow the CRISP_DM framework to do the data analysis. The analyzing notebook is located at
https://github.com/crystallljjj/krafwerk/blob/ML/AI_task11/prompt_II.ipynb

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


      which state has more used car?
      plot the car number based on the state. We can see that California has most used car.
      ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/082e918c-d25d-421d-859f-9996a38440fc)

      Group the data by 'manufacturer'. The most popular three brands are "ford", "chevrolet" and "toyota".
    
      ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/3f065b80-e1c6-45cb-b485-8d536e5caa0c)

      Classify the data by the 'fuel' and plot the ratio below.
      ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/00af454f-6cab-4a44-8cf9-964ddcf61146)

      Group the data by "drive" and plot the ratio.
      ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/ef9cf3a2-8aaa-4cf7-8b6e-f5c7aa61698e)

      Group the data by 'type' and plot the mean price for each type.
      Pickup has highest price in all types of 'car'.
      ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/df9a64f0-746b-4c50-a239-dd5f0c76d56d)

   
 4. Data preparation
     Since the used car price is varies a lot based on the location. Next, we will pick up "California" data to analyze. Besides, since "size" has a very high ratio N/A value, we drop this column. We also drop "VIN", "id", "region" columns and N/A.
    
      For cross validation, we split the data into two set. X_train(80%), X_test(20%)
     ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/4529f859-b910-4617-aa80-a5197040f973)


  5. Modeling
   First, build a Linear regression model
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/ca30a0df-372b-42bf-be4f-d59f1328127c)
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/9b46d832-31a8-4e44-9cb5-68ecb92f8d26)

   Second, build a Ridge model.
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/fd213568-5131-40b3-83af-421521d90a01)
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/dde0182b-5642-414f-afdc-380e7666f8fd)

   Third, analyze the permutation importance of the cloumns
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/7b3b4fab-e99a-4f1e-b66f-1ac21012b92a)

   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/eb8a0a86-8c49-40be-9270-5cf5e01fc9d9)


  5. Evaluation
     # After the testing above, it shows that 'type', 'model', 'drive' and 'fuel' are the most important factors affecting the used car price.
# All the features above will lead user to select one type of car. When the type of car is selected, 'year', 'manufacturer', 'condition' , 'paint_color' and all other factors will affect the price of the car.        




