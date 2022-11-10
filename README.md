# Neural_Network_Charity_Analysis
______________________________________________________________________________
## Overview of the analysis: Explain the purpose of this analysis.
______________________________________________________________________________

The purpose of the project is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by the cilent  Alphabet Soup. From Alphabet Soup’s business team, the team will utilize a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The goal of the project is to determine the classification of any future organizations wishing to use the cilent's services


## Results: Using bulleted lists and images to support your answers, address the following questions.
____________________________________________________________________________________________________________
  ### Data Processing 
    1. What variable(s) are considered the target(s) for your model?

    The target of IS_SUCCESSFUL is currently the only target for the model.
_____________________________________________________________________________________________
    2. What variable(s) are considered to be the features for your model?

       * APPLICATION_TYPE
       * AFFILIATION 
       * CLASSIFICATION 
       * USE_CASE 
       * ORGANIZATION
       * STATUS
       * INCOME_AMT
       * SPECIAL_CONSIDERATIONS
       * ASK_AMT 
  
  are the variables we want to explore in relation to the binary success, or non-success of the org.
__________________________________________________________________________________________________________    

    3. What variable(s) are neither targets nor features, and should be removed from the input data?
      * EIN 
     * NAME 
  
  have been removed because they are only used for identification.
______________________________________________________________________________________________________
 ### Compiling, Training, and Evaluating the Model

    4. How many neurons, layers, and activation functions did you select for your neural network model, and why?
   On the first attempt, I created a model with 2 hidden layers (6 neurons in the first, 3 neurons in the second), using activation "relu" and "sigmoid". 
    

### 5. Were you able to achieve the target model performance?

### 6. What steps did you take to try and increase model performance?

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
