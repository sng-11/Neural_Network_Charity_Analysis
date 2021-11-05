# Neural Network Charity Analysis: Alphabet Soup

## Overview of Analysis
Our client, AlphabetSoup, is interested in investing in charitable organizations. In order to appropriately allot their investments, they would like to use machine learning to predict the success of those charities if they received funding from AlphabetSoup. For this endeavor, a neural network model will be used to analyze data of 34,000 organizations. The platform used is TensorFlow in Python.

## Results

### Data Preprocessing
- Target Variable: __IS_SUCCESSFUL__ is the target because it contains binary data indicating whether money was used effectuvely. Ultimately, this is the information that our client would like to predict.
- Features of the Model: __APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT__
- The variables that should be removed: __EIN__ and __NAME__ because identification information is not needed to predict the outcome of funding the charity.

### Compiling, Training, and Evaluating the Model
- 
