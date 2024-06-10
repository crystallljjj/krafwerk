## Overview:
In this third practical application assignment, the goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) you encountered in this section of the program. You will use a dataset related to the marketing of bank products over the telephone.

## Data:
The dataset comes from the UCI Machine Learning repository Links to an external site.The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. https://archive.ics.uci.edu/dataset/222/bank+marketing

## Start to process the data
### load the data
data = pd.read_csv('bank+marketing/bank/bank.csv',sep = ';')
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/117aee6c-e85a-4485-8a16-577a0355235d)
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/1d33aa2a-728c-4e08-b9bd-f4ec6fafef3d)

explore the categorical columns
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/13a325f9-495f-406f-9fca-1c4f45f67578)

explore the numerical columns
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/9129b69a-c332-488e-bb63-a9bc9fd273f6)


### preprocessing the data/encode the 'str' to 'num'
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/84d1fa4a-2ac4-472b-9e69-ab3d3d32f75e)
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/54c8a7c3-f31b-43c6-af43-ad7a60572527)

### split the data to testing set and trainning set
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/71f8222d-2e7b-4ef3-b6bc-a51804bfdf37)

### train the dataset with different models and compare the results
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/39fd0401-deda-4250-9b9a-df6e135090ef)

### the trainning results
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/4affc51a-4673-4008-9fc6-5c5fd4625483)

![image](https://github.com/crystallljjj/krafwerk/assets/14128797/1d9000ea-f424-400b-bc21-cc7095328af5)
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/7bf3076b-7c52-4c22-a2b7-28515bc256b4)
![image](https://github.com/crystallljjj/krafwerk/assets/14128797/f063ff2d-479d-4024-a731-ce6c5852f9d5)

### conclusion
Based on the analysis above, we found that using this dataset, the accuracies of different models don't have a large different. But the fitting time, since the complex of the algorithm have obvious differnces.

KNN method has shortest fitting time.

Desicsion tree methods is a little bit longer than KNN, but still is efficient.

SVM methos have more than 200 times larger fitting time, which in this case, is not a efficient solution.
