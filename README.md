The project is analyzing and building the model to predict the breast cancer wisconsin (diagnostic). The data is coming from https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data.
The reason why I chose this dataset is considering the medical detection is a good area to apply the machine learning algorithm. It could help doctor to detect the disease fast and understand more about it. It could also provide a database to develop artificial fast detection to helper customer fast filter disease. The medical area will become a fast growth inductry of AI/ML application.

1. Load the data and explore the data properties
   This dataset contains 32 columns and 569 rows.
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/b95b0aef-f04b-48ec-a524-ff600448ca74)

   1.1 plot the distribution of each data column
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/f1f08db7-ead9-4c22-b4ab-cc2d45fca1e0)
    ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/65c1b530-8df6-4c54-973b-237826ff52c7)

   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/c95262a3-fedc-42da-a060-da44243d44fa)
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/32cab56f-667d-4af8-be34-ca3b39fa5105)

   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/cae700e0-33bf-4b84-965e-03de4d1c06f4)

   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/f88de722-b093-437d-bd46-9cfcb29cb1bc)
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/c21ee2db-2e57-4ea1-b6cb-2f68243e5af2)

   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/2e529b65-4231-4ffa-811d-b45eee9d3ea2)

  ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/1679ac32-1e05-4e17-ab4d-8a285f786342)

  1.2 plot the heatmap of of the correlation between columns
  ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/b5890a97-7334-4f9d-a592-00f5f077b354)

2. Preprocessing and split data
   Since the data has different ranges, we apply a normoalization to the raw data.
   And spli the data to be a training set and a testing set.
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/3954089e-74e5-4d8c-892a-38be2552b38d)

   
3. Create a list of models to train the data
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/33a2bf46-4c1e-4945-8b9e-ca4642071222)

5. Train the model and plot the results
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/31b8b92d-6a16-40d0-867e-ff10d9320a8d)
   Based on the results, logistic regression gives best accuracy. 
6. Hyperparameter tuning for logistic regression
   ![image](https://github.com/crystallljjj/krafwerk/assets/14128797/52fd70e7-8fda-4c66-a1fb-afcf9a09d35d)

7. Fitting results. (The best model)
## The best model for this dataset is LogisticRegression. 
## The best parameters are C = 10, penalty = l2
## The cross-validataion accuracy is 0.9495
