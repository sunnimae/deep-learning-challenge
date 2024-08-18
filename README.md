Neural Network Model
This model is designed to predict whether applicants will be sucessful if funded by Alphabet Soup.

The variable target is: IS_SUCCESSFUL

The feature variables are: NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERTIONS, ASK_AMT.
The variables that are neither targets nor features, and was therefore removed is the identification columns (EIN).

The inital attempt to build the model yield only 72.4% accuracy. On the first attempt, I removed EIN and NAME columns. This approach resulted in a limited number of variants for the model to work with, leading to low accuracy.

After consulting with tutor Khangwelo, I reintroduced the NAME column, and reduced the number of unique values from 19568 to 355. The second attempt improved the accuracy from 72.4% to 78.9% and decreased the loss from 0.55 to 0.44.

Summary:
Although the accuracy increased to 78.9%, it is still not high enough for real world applications. Therefore, I recommend using a different model. 
The model I propose is Random Forest, mainly due to the size and the type of the dataset. 
Random Forests are quick to train and to optimize according to their hyperparameters [3]. Thus, the computational cost and time of training a Random Forest are comparatively low. (source: https://blog.frankfurt-school.de/wp-content/uploads/2018/10/Neural-Networks-vs-Random-Forests.pdf) 
