# Neural_Network_Charity_Analysis
![Neural Network Photo](https://user-images.githubusercontent.com/87907584/146254740-d03d159a-0eca-4fef-ad4c-2ae1c3853064.PNG)

## Overview of the analysis: Explain the purpose of this analysis.
AlphabetSoup is looking for a learning model that will effectively predict if applicants will be successful by being funded. 

# Data Preprocessing
- What variable(s) are considered the target(s) for your model? <br>
The IS_SUCCESSFUL variable is considered the targed for the model.<br>
- What variable(s) are considered to be the features for your model?<br>
The following variables were initially considered to be the feaures of our model. APPLICATION_TYPE, AFFILIALTION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT.  
- What variable(s) are neither targets nor features, and should be removed from the input data?<br>
Variables EIN and NAME were dropped in the original dataset, however we added the NAME variable in our optimization file. 

# Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
For optimization we finally landed on 3 hidden layers keeping the ratio of neurons per hidden layer of 1 to 2 the deeper we layered. 
- Were you able to achieve the target model performance?
After much trial and error and support I was able to surpass the targed model perfromance reaching 77%... FINALLY!
- What steps did you take to try and increase model performance?
Initially, I recognized the insignificant columns that we could remove. Binning was updated as well as the activation type.  We initially used relu, however, it is suggested that when a model does not train as intended, to use a stronger model.  For optimization, both relu was replaced with sigmoid.<br> 

# Summary<br> 
- Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation. <br>
When using the initial code provided, accuracy stalled around 72 to 73 percent.  Finally, when the NAME was reintroduced back into the dataset as well as binning outliers, adding additional layers, I was able to reach the target model performance. 
