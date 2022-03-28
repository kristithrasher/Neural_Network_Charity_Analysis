# Neural_Network_Charity_Analysis

## Overview
Alphabet Soup is a foundation asking for help to predict where to make investments.
Working with Beks, from the data analyst team, we are asked to use knowledge of machine learning and neural networks, and to help Beks create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. 
We were provided a dataset in csv format and will use Pandas and the Scikit-Learn libraries to perform the following analysis.
Purpose is to predict whether applicants will be successful if funded by Alphabet Soup. 
## Results
* Data Preprocessing
* Preprocessing Data for a Neural Network Model
*Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your  dataset:
  	*IS_SUCCESSFUL variable is the target(s) for our model.
 	 *The following variables are considered the features for our model. 44 total. 
STATUS                            
ASK_AMT                           
IS_SUCCESSFUL                     
APPLICATION_TYPE_Other          
APPLICATION_TYPE_T10            
APPLICATION_TYPE_T19            
APPLICATION_TYPE_T3             
APPLICATION_TYPE_T4             
APPLICATION_TYPE_T5             
APPLICATION_TYPE_T6             
APPLICATION_TYPE_T7             
APPLICATION_TYPE_T8             
AFFILIATION_CompanySponsored    
AFFILIATION_Family/Parent       
AFFILIATION_Independent         
AFFILIATION_National            
AFFILIATION_Other               
AFFILIATION_Regional            
CLASSIFICATION_C1000            
CLASSIFICATION_C1200            
CLASSIFICATION_C2000            
CLASSIFICATION_C2100            
CLASSIFICATION_C3000            
CLASSIFICATION_Other            
USE_CASE_CommunityServ          
USE_CASE_Heathcare              
USE_CASE_Other                  
USE_CASE_Preservation           
USE_CASE_ProductDev             
ORGANIZATION_Association        
ORGANIZATION_Co-operative       
ORGANIZATION_Corporation        
ORGANIZATION_Trust              
INCOME_AMT_0                    
INCOME_AMT_10000-24999          
INCOME_AMT_100000-499999        
INCOME_AMT_10M-50M              
INCOME_AMT_1M-5M                
INCOME_AMT_25000-99999          
INCOME_AMT_50M+                 
INCOME_AMT_5M-10M               
INCOME_AMT_Jan-99               
SPECIAL_CONSIDERATIONS_N        
SPECIAL_CONSIDERATIONS_Y        
 
  * Preprocessed the dataset:  We used Pandas and the Scikit-Learn’s StandardScaler(). Scikit-Learn's StandardScaler() was used to standardize the numerical data such that the variables were rescaled to a mean of 0 and standard deviation of 1. Once the data was standarized we were able to transform and standardize the dataset. Once we had our transformed data within the StandardScaler instance, we exported the transformed data into a Pandas Dataframe and passed to our neural network model 


* Compile, Train, and Evaluate the Model
* The neural network model using TensorFlow Karas contains working code that performs the following steps:
1.	We used 3 layers (input, hidden, and output), We had 80 number of neurons in input layer, 30 in the hidden layer, The rule of thumb is to have the amount of input variables x2 or 3 for you number or neurons. The activation function we used for input and hidden layers was the ReLU function. it returns a value from 0 to infinity, it is the most common and is default function. We used the sigmoid funciton for our output layer becasue it determines probability and transforms output to a range between 0 and 1. 


2.	An output layer with an activation function is created ouput from structure of model.
![structure of model](https://user-images.githubusercontent.com/94208810/160459328-de1c2cb2-1dd3-48e7-92b8-eda70ade1e95.png)

3.  There is an output of the model’s loss and accuracy 

![deliv1lossAccuracy](https://user-images.githubusercontent.com/94208810/160459076-08e093d4-76ab-40c3-8604-9e31114e5725.png)



5.	The model's weights are saved every 5 epochs 

![epoch5](https://user-images.githubusercontent.com/94208810/160459057-3e197631-794e-4b00-b6b1-1327a5da1ba5.png)


6.	The results are saved to an HDF5 file AlaphabetSoupCharity_Optimization.h5.
![output](https://user-images.githubusercontent.com/94208810/160459953-02648c27-db6b-4874-b011-94dafa1cb1d8.png)


 
* Optimize the Model (did one of these by creating 3 different attempts)
* Here are a few means of optimizing a neural network:

First Attempt: 
Noisy Variables are removed from features(“STATUS” and “SPECIAL_CONSIDERATIONS”
Added 30 more neurons to a hidden layer2. 
Models weights are saved every 5 epochs. 
Output showed a decrease in accuracy so no benefit of accuracy at .7247. 
![optimization attempt1](https://user-images.githubusercontent.com/94208810/160460432-f0273e4b-52ce-4857-a300-65741bd7c1bc.png)
 

Second Attempt: 
Added 40 more neurons to a hidden layer1 and kept hiddenlayer2 at 60. 
Use a different activation function for the hidden layers from “ReLU” to “Sigmoid”. 
Add additional epochs to the training regimen by increasing from 100 epochs to 150.
Models weights are saved every 5 epochs. 
The accuracy was lower than original with these changes so no benefit to my changes with accuracy at .72489


Third Attempt: 

Added  additional hidden layers with activation function of “ReLU” and neurons at 30.
Add additional epochs to the training regimen by increasing from 100 epochs to 200. 
Models weights are saved every 5 epochs. 
The accuracy increased mildly from original with a accuracy of .7261
![optimizationattempt3](https://user-images.githubusercontent.com/94208810/160460342-b03c1438-a03a-4d2d-9389-3512f679730d.png)

## Summary
The overall results of the deep learning model and the recommendations I have for how a different model that could solve this classification problem would be decision trees, random forests, and gradient-boosted trees because they are used to solve classification problems.

