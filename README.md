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

3. What variable(s) are neither targets nor features, and should be removed from the input data?
   * EIN 
   * NAME 
  have been removed because they are only used for identification.
______________________________________________________________________________________________________
 ### Compiling, Training, and Evaluating the Model
 
4. How many neurons, layers, and activation functions did you select for your neural network model, and why? 
For the initial attempt at model, two layers, with 80 and 30 neurons respectively (both "relu" type) were used. The activation feature of "sigmoid" was used. This was presented by the client as the starting point for model creation, allowing the analyst two further adjust in order to increase optimization.
    

5. Were you able to achieve the target model performance? 
The model performance was set at 75%. Unfortunately, the current model only achieved an accuracy rating of 74.09% on epochs 96 and 99. An overall accuracy average of 72.98% was achieved.

6. What steps did you take to try and increase model performance?

  Attempt 1:

    Dropped noisy data of ASK_AMT
    Hidden layer one: tanh type - 80 neurons
    Hidden layer two: relu type - 30 neurons
    Activation: sigmoid
    Highest accuracy/epoch: 74.08%, epoch 81 of 100
    Overall accuracy average: 72.79%

   Attempt 2:

    Dropped noisy data of ASK_AMT
    Hidden layer one: tanh type - 80 neurons
    Hidden layer two: relu type - 50 neurons
    Hidden layer three: sigmoid type - 30 neurons
    Activation: relu
    Highest accuracy/epoch: 74.00%, epoch 89 of 100
    Overall accuracy average: 73.04%

  Attempt 3:

    Dropped noisy data of ASK_AMT
    Hidden layer one: sigmoid type - 100 neurons
    Hidden layer two: sigmoid type - 75 neurons
    Hidden layer three: relu type - 50 neurons
    Hidden layer four: relu type - 25 neurons
    Activation: sigmoid
    Highest accuracy/epoch: 74.09%, epoch 99 of 100
    Overall accuracy average: 72.92%

  Attempt 4:

    Dropped noisy data of ASK_AMT
    Hidden layer one: sigmoid type - 60 neurons
    Hidden layer two: relu type - 30 neurons
    Hidden layer three: relu type - 15 neurons
    Activation: sigmoid
    Highest accuracy/epoch: 74.20%, epochs 155 and 162 of 200
    Overall accuracy average: 72.47%


## Summary: 
the above detail illustrates the ill performanc of the model- 72% accuracy with little improvement gained with multiple adjustments, the initial setup for the model did not perform at the required level,  72.98%. Multiple turnsachieved an increased rating of 73.04% on the second optimization attempt. All other models had lower final accuracies than the initial model. For this, it can be seen that changing the number of hidden layers and neurons had a negligible effect on increasing model accuracy. continued manipulation might invalidat the or prove it infeasible to present to the client as a viable source of informantion.

Further analysis may prove frituful if permitted to continue testing utilizing additonal resources and alternative modeling.

