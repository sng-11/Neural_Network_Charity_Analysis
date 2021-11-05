# Neural Network Charity Analysis: Alphabet Soup

## Overview of Analysis
Our client, AlphabetSoup, is interested in investing in charitable organizations. In order to appropriately allot their investments, they would like to use machine learning to predict the success of those charities if they received funding from AlphabetSoup. For this endeavor, a neural network model will be used to analyze data of 34,000 organizations. The platform used is TensorFlow in Python.

## Results

### Data Preprocessing
- Target Variable: __IS_SUCCESSFUL__ is the target because it contains binary data indicating whether money was used effectuvely. Ultimately, this is the information that our client would like to predict.
- Features of the Model: __APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT__
- The variables that should be removed: __EIN__ and __NAME__ because identification information is not needed to predict the outcome of funding the charity.

### Compiling, Training, and Evaluating the Model
- In the initial attempt to create a neural network model, there were 2 hidden layers (80 and 30 neurons respectively), with only 0.68 accuracy. The activation function chosen was ReLU for the hidden layers because ReLU can speed up training (as its gradient composition is either 0 or 1). With binary classification, Sigmoid is chosen for the output layer. 
- To optimize, the first attempt made was to add neurons to the first hidden layer (from 80 to 100). The other properties were kept the same. The accuracy score from the change was negligibly improved, at 0.69. 
- The second attempt to optimize involved binning any additional values. The ASK_AMT column was binned. However, even when the first hidden layer had 100 neurons, the accuracy was 0.64 which was lower than previous attempt.
- The third attempt to optimize involved adding a third hidden layer. The hidden layers therefore now compose of 80, 30, and 30 neurons. Unfortunately, the accuracy score is only 0.63.

### Summary
Despite multiple attempts at optimization, the machine learning neural network did not reach 75% accuracy. Since this problem requires binary classification, another model that can be trialed is the Random Forest Classifier. 
