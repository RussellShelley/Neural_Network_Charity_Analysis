# Neural_Network_Charity_Analysis

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions.

Data Preprocessing
What variable(s) are considered the target(s) for your model?
What variable(s) are considered to be the features for your model?
What variable(s) are neither targets nor features, and should be removed from the input data?
Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?
 

## Overview


We are creating a neural network that will act as a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
We will train and test the neural network on data provided in a CSV which contains information on more than 34,000 organizations that have received funding from Alphabet Soup over the years. This data will be preprocessed, eliminating useless variables, encoding categorical data, and scaling values. We will adjust our model to see if we can raise our models accuracy above 75%.

## Resources


## Results
- Data Preprocessing
     - For this model we are trying to find out if an organization is going to be successful, so out target variable will be the binary "IS_SUCCESSFUL" values. 


    - The following variables are our models features:
        - APPLICATION_TYPE—Alphabet Soup application type,
        - AFFILIATION—Affiliated sector of industry
        - CLASSIFICATION—Government organization classification
        - USE_CASE—Use case for funding
        - ORGANIZATION—Organization type
        - STATUS—Active status
        - INCOME_AMT—Income classification
        - SPECIAL_CONSIDERATIONS—Special consideration for application
        - ASK_AMT—Funding amount requested
    

    - We can drop "EIN" and "NAME" as these are just columns used to identify the individual organizations. 

    - I created a bin for "APPLICATION_TYPE", that collects types that appear less than  500 times into a new  other category. I did the sam for "CLASSIFICATION" (less than 1800).
    This reduced the number of categories to 9 and 6 respectively.
    - I then used One hot encoder, to encode our categorical data as a one-hot numeric array.
    - The processed data was then split X_train, X_test, y_train, y_test.
    - The feature data was scaled using standardscaler. (data is given a new mean of 0 and SD of 1)


- Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - For my model I decided to start with two hidden layers. 
    - The number of neurons in the first hidden layer should be less than the inputs and more than the output. I decided to use 8 in the first layer, and 5 in the second. We have just one output.
    - The activation function I decided to use on my hidden layers is "reLu", Rectified Linear Unit. It is used a lot and seems to be the default activation function for neural networks. 
    - I used a "sigmoid" activation function on my output layer.  Sigmoid works well for binary output.
    - The model ran for 100 epochs.


- Were we able to achieve the target model performance?
    - This model achieved  **73% accuracy**. Not the 75 % we were hoping for!

- Increasing model performance
    - 



## Summary

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.