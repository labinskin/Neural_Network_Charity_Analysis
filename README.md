# Neural_Network_Charity_Analysis

### Background

Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- **EIN** and **NAME**—Identification columns
- **APPLICATION_TYPE**—Alphabet Soup application type
- **AFFILIATION**—Affiliated sector of industry
- **CLASSIFICATION**—Government organization classification
- **USE_CASE**—Use case for funding
- **ORGANIZATION**—Organization type
- **STATUS**—Active status
- **INCOME_AMT**—Income classification
- **SPECIAL_CONSIDERATIONS**—Special consideration for application
- **ASK_AMT**—Funding amount requested
- **IS_SUCCESSFUL**—Was the money used effectively



### Results

- Data Preprocessing
  - What variable(s) are considered the target(s) for your model?
  - ![]()
  - The target is IS_SUCCESSFUL, either a 0 or 1 as binary data.
  - What variable(s) are considered to be the features for your model?
  - ![]()
  - The features are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
  - What variable(s) are neither targets nor features, and should be removed from the input data?
  - ![]()
  - The variables that were dropped as neither targets nor features were NAME and EIN.
- Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - ![]()
  - In the original neural network, there were two hidden layers of 80 and 30 neurons, and one output layer. The two hidden layers had "relu" activation functions, with the output layer having "sigmoid" as its activation. This original model also ran for 100 epochs.
  - ![]()
  - ![]()
  - My neural network had four hidden layers, with 80, 50, 25, and 15 neurons respectively. Each of their activation functions was "relu". There was one output function, with its activation set as "sigmoid." This model ran for 200 epochs. These choices were made after a series of trials and errors. The model with four hidden layers and 200 epochs was the closet to achieving the 75% model target performance However, there could have been a possible reduction in epochs from 200 to 150, with only a minor difference in overall outcome.
  - Were you able to achieve the target model performance?
  - ![]()
  - No, while the final epoch has an accuracy of 74.61%, which could be rounded up to 75%, the overall model accuracy is just 73.02%, falling below the 75% threshold.
  - What steps did you take to try and increase model performance?
  - ![]()
  - ![]()
  - In addition to the extra neurons, layers, and epochs as noted above, there was one category, ASK_AMT, that had an unusually high number of different inputs (8747). I decided to bin these inputs to see if this would help increase model performance. And while all of these steps did increase the accuracy compared to the original accuracy (see image below), it still did not reach the threshold.

### Summary
