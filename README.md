# Neural_Network_Charity_Analysis

## Overview of the analysis
We were assigned the task of using the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. In order to complete the task, we first needed to preprocess the dataset in order to compile, train, and evaluate the neural network model. After the dataset was preprocessed, we designed a neural network/deep learning model to create a binary classification model that can predict if the organization will be successful based on the feature of the dataset. Once the numbers of neurons and layers were determined, we compiled, trained, and evaluated the binary classification model to calculate the model's loss and accuracy. Lastly, we were to optimize the model in order to acheive a target predictive accuracy higher than 75%. 

## Results: Using bulleted lists and images to support your answers, address the following questions.
Data Preprocessing</br>
1. What variable(s) are considered the target(s) for your model?</br>
The IS_SUCCESSFUL column was considered the target for our model. This column determined whether the organization fund was used effetively or not. 
2. What variable(s) are considered to be the features for your model? </br>
The following columns were considered to be the features for our model: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. 
3. What variable(s) are neither targets nor features, and should be removed from the input data?</br>
The two columns that were removed from the dataset was EIN and NAME. The two columns were used for identification purposes. </br></br>

Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why?</br>
The deep learning neural network model consists of two hidden layers with 150 and 75 neurons. This model resulted in an accuracy of 71%.</br>
![deeplearning_evaluation](https://github.com/echuung94/Neural_Network_Charity_Analysis/blob/main/Resources/deeplearning_evaluation.png)</br>

To improve the accuracy of the model, a third hidden layer was added. Adding an additional layer resulted in an accuracy of 70%, which was not effective in achieving the target model performance rate of 75%. </br>
![thirdlayer_evaluation](https://github.com/echuung94/Neural_Network_Charity_Analysis/blob/main/Resources/thirdlayer_evaluation.png)</br>

A different activiation function was used to improve the neural network model. Tanh was used in place of Relu and resulted in an accuracy of 70% as well. </br>
![tanh_evaluation](https://github.com/echuung94/Neural_Network_Charity_Analysis/blob/main/Resources/tanh_evaluation.png)</br>

2. Were you able to achieve the target model performance?</br>
Adding the additional hidden layer and using a different activation function was not effective in increasing the accuracy level of 75%. The following trials did not show a positive performance in predicting if the charity donations were successful or not. </br>

3. What steps did you take to try and increase model performance?</br>
Initially, the number of neurons were increased to try and increase model performance. A third hidden layer was also added to increase the performance of the neural network model. Both models failed to acheieve the target performance. Lastly, the activation function of the model was changed to try to increase model performance, but the change in function also failed to improve the performance rate. 

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
After trials and errors, the deep learning neural network model was unsuccessful in reaching the target model performance rate of 75%. In order to improve performance, I would recommend using the Random Forest Classifier. The Random Forest model combines multiple smaller models into a more accurate model. It would be faster to train due to this model being able to easily work with multiple features. 
