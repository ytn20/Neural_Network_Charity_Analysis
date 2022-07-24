# Neural_Network_Charity_Analysis

# Overview of the loan prediction risk analysis:

The purpose of this analysis is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. In this project we will analyze over 10 columns that capture metadata about each organization that has received funding from Alphabet Soup. The columns contain identification details, application type, use case, status, income classification and more. Using Artificial Neural Networks we will be able to help the foundation predict where to make investments.

Below is a detailed list of all columns within this dataset

- **EIN and NAME** — Identification columns
- **APPLICATION_TYPE** — Alphabet Soup application type
- **AFFILIATION** — Affiliated sector of industry
- **CLASSIFICATION** — Government organization classification
- **USE_CASE** — Use case for funding
- **ORGANIZATION** — Organization type
- **STATUS** — Active status
- **INCOME_AMT** — Income classification
- **SPECIAL_CONSIDERATIONS** — Special consideration for application
- **ASK_AMT** — Funding amount requested
- **IS_SUCCESSFUL** — Was the money used effectively

# Results:

## Data Preprocessing
- What variable(s) are considered the target(s) for your model?
The variable that was considered the target variable for this model was the "IS_SUCCESSFUL" column.

- What variable(s) are considered to be the features for your model?
The variable that were considered the features for this model were all columns expect the "IS_SUCCESSFUL" column.

- What variable(s) are neither targets nor features, and should be removed from the input data?
In this dataset two variables were considered nor targets or features and hence were removed from the input data in the Data Preprocessing portion of the analysis. The two variables that were dropped were the identification columns - "EIN" and "NAME" columns.

![2](https://user-images.githubusercontent.com/100486461/180670615-10233fe4-07f9-4ae6-aa97-8374315487bd.PNG)
![3](https://user-images.githubusercontent.com/100486461/180670614-b3d2f79c-cb36-472f-a062-a55baecdd8e3.PNG)

## Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
For my neural network model I selected 2 hidden layers (hidden_nodes_layer1 and hidden_nodes_layer2). Where hidden_nodes_layer1 has 80 neurons and hidden_nodes_layer2 had 30 neurons. The activation function for the two hidden layer was Relu function and the activation function I chose for output layer was Sigmoid function.
![4](https://user-images.githubusercontent.com/100486461/180670711-27b0f7cd-55db-4cfb-b507-8b5b1af0204d.PNG)

- Were you able to achieve the target model performance?
I was unable to reach the 75% target model performance with this model. My accuracy score for the model was approximately 72%
![1](https://user-images.githubusercontent.com/100486461/180670725-a3e588b8-6ef0-4ebc-a558-0f54814a85c6.PNG)

- What steps did you take to try and increase model performance?
I attempted to improve the model performace with three models where I increased the ammount of hidden layers, the amount of neurons for each layer as well as tried to use different activation function and was unable to increase the model performace. The final accuracy score for my model was approximately 72.05%. 

![m1](https://user-images.githubusercontent.com/100486461/180670731-574d42a7-f4b9-45c3-a710-71fc2a91285c.PNG)
![m2](https://user-images.githubusercontent.com/100486461/180670732-4686447b-2242-4aac-a06b-0042126dcab3.PNG)
![m3](https://user-images.githubusercontent.com/100486461/180670730-43b726f2-e257-4bd2-8334-5c149220895f.PNG)
![m3s](https://user-images.githubusercontent.com/100486461/180670787-a30e7773-e2f3-433c-a84b-e9dc6f50bae0.PNG)

# Summary:

Overall the model accuracy score did not improve even after the optimization. The initial model accuracy score was 72% and the final model accuracy score was approximately 72.05%. The reason for this could be that the model is overfitted. In order to increase the model performance we can try running Random Forest Classifier as it can help combine different smaller models into a more robust and accurate model.


![1](https://user-images.githubusercontent.com/100486461/180670628-3583122a-f51c-48f3-95cf-7cb37d2d3752.PNG)
![m2s](https://user-images.githubusercontent.com/100486461/180670762-2ce510b1-b47c-4365-8a72-34802e8de8fd.PNG)
![m3s](https://user-images.githubusercontent.com/100486461/180670758-364ec289-dc02-4b8a-8ffa-2ebb3dea7f30.PNG)
