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
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

## Overview


We are creating a neural network that will act as a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
We will train and test the neural network on data provided in a CSV which contains information on more than 34,000 organizations that have received funding from Alphabet Soup over the years. This data will be preprocessed, eliminating useless variables, encoding catergorical data, and scaling values. We will adjust our model to see if we can raise our models accuracy above 75%.

## Resources


## Results
- Data Preprocessing
What variable(s) are considered the target(s) for your model?
    - For this model we are trying to find out if an organization is going to be successful, so out target variable will be the binary "IS_SUCCESSFUL" values. 

What variable(s) are considered to be the features for your model?
    -
What variable(s) are neither targets nor features, and should be removed from the input data?
    - We can drop "EIN" and "NAME" as these are just columns used to identify the individual organizations. 
Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Were you able to achieve the target model performance?
- What steps did you take to try and increase model performance?



## Summary