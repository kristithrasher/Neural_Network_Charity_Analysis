# Neural_Network_Charity_Analysis

## Ovwerviewour
Alphabet Soup, is a foundation asking for help to predict where to make investments.
Working with Beks, from the data analyst team, we are asked to use knowledge of machine learning and neural networks,  and to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 
We were provided a dataset in csv format and will use Pandas and the Scikit-Learn’s libraries to perform the following analysis.
## Analysis
* Preprocessing Data for a Neural Network Model
  *Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your        dataset:
  *What variable(s) are considered the target(s) for your model?
  *What variable(s) are considered the feature(s) for your model?
  *Drop the EIN and NAME columns.
  *Determine the number of unique values for each column.
  *For those columns that have more than 10 unique values, determine the number of data points for each     unique value.
  *Create a density plot to determine the distribution of the column values.
  *Use the density plot to create a cutoff point to bin "rare" categorical variables together in a new      column, Other, and then check if the binning was successful.
  *Generate a list of categorical variables.
  *Encode categorical variables using one-hot encoding, and place the variables in a new DataFrame.
  *Merge the one-hot encoding DataFrame with the original DataFrame, and drop the originals.
  
  * Preprocessed the dataset:  We used Pandas and the Scikit-Learn’s StandardScaler(). Scikit-Learn's StandardScaler() was used to standardize the numerical data such that the variables were rescaled to a mean of 0 and standard deviation of 1. Once the data was standarized we were able to transform and standardize the dataset. Once the we had our transformed data within the StandardScaler instance, we exported the transformed data into a Pandas Dataframe and passed to our neural network model 



* Compile, Train, and Evaluate the Model
 
* Optimize the Model

## Summary
