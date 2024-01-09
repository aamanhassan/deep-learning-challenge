# deep-learning-challenge
Module 21

The report should contain the following:

# Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

# Data Preprocessing

1. What variable(s) are the target(s) for your model?

  **Answer** : The target is the IS_SUCCESSFUL column.

2. What variable(s) are the features for your model?

  **Answer** : Features list are the following: NAME, APPLICATION_TYPE,AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT,    SPECIAL_CONSIDERATIONS, ASK_AMT.

3. What variable(s) should be removed from the input data because they are neither targets nor features?

  **Answer** :EIN(Employee identification number)


# Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

  **Answer** : In this module, we implemented a neural network with three hidden layers, each featuring a substantial number of neurons. This choice was driven by the observed improvement in accuracy, surpassing 75% and reaching around 79%,although it comes with increased computational costs. First activation is rulu and the rest two are sigmoids, as it might boost accuracy level.
  I also enhanced my dataset by incorporating categorical names and applying encoding to get dummies. This adjustment is anticipated to contribute to improved model scores.

2. Were you able to achieve the target model performance?

  **Answer** : Yes

3. What steps did you take in your attempts to increase model performance?

  **Answer** : It was beneficial to transform the "NAME" feature into data points to maximize efficiency, although this process incurs higher costs. Additionally, introducing a third hidden layer with a sigmoid activation function is deemed necessary to further enhance the model's performance.

#Summary: Summarize the overall results of the deep learning model.

In summary, the deep learning model achieved an overall accuracy exceeding 75%, demonstrating its ability to correctly classify applicants in the test set 75% or more of the time. Moreover, an interesting insight emerged from the analysis, indicating that applicants have an 80% chance of success if they fulfill specific criteria:

The applicant's name appears more than 5 times.
The application type falls within the categories T3 T4 T5 T6 T7 T8 T9 T10 or T19.
The application aligns with specific classifications C1000 ,C2000 ,C1200 , C2100, C3000 


#Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

RandomForest model


