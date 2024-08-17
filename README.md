Neural Network Model
This model is build to predict whether applicants will be sucessful if funded by Alphabet Soup.

The variable target is: IS_SUCCESSFUL

The feature variables are: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERTIONS, ASK_AMT.
The variables that are neither targets nor features, and were therefore removed are the identification columns (EIN and NAME).

To increase the the accuracy of the results, I have tried the following to optimize the model.
Image_1 : Combination of activation functions Tanh(86 units) -Tanh (86 units) -Sigmoid (1 unit), epoch 50. Accuracy Rate is 72.4%
Image_2:  Combination of activation functions Relu(86 units) -Relu (86 units) -Sigmoid with epoch 50. Accuracy rate is 72.4%
Image_3:  Three hiddenlayers, with activation function Relu(30 units in each layer) and a Sigmoid activation (Unit 1) in the output layer. With 20 Epochs, the accuracy rate is still 72.4%

I was not successful in achieving the target model performance at 75%.

For experimentation, I also used Keras Tuner to explore different hyperparameters to see if a better accuracy rate could be achieved.
After running Keras Tuner for 21 minutes, it appears that the peak performance of this model is in the range of  72.4% - 72.6%. The Keras Tuner search results can be found in tuner_search_image.

Summary:
The dataset for the Neural Network Model in question might be too small. The next model I would try would be the Random Forest, as it can handle both categorical and numerical features effectively and provides feature importance insights.
