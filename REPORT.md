# Module 21 - Deep Learning Challenge

## Report on the Neural Network Model

1. Overview of the analysis:
Alphabet Soup, a nonprofit charitable foundation is in need of a tool that can help them select the applicants for funding with the best chance of success in their ventures. With provided dataset from Alphabet Soup's business team, I have been able to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

The dataset was provided in a CSV containing more than 34,000 organisations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organisation,

2. Results: 
Data Preprocessing
- What variable(s) are the target(s) for your model?
The target variable is the 'IS_SUCCESSFUL' column from application_df

- What variable(s) are the features for your model?
All column in the dataset application_df are the features variables except the 'IS_SUCCESSFULL'.

- What variable(s) should be removed from the input data because they are neither targets nor features?
Both 'EIN' and 'NAME' columns were removed because they were neither targets nor features for the dataset.

#### Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
On the first attempt (AlphabetSoupCharity.ipynb), first hidden layer with 80 neurons and second hidden layer with 30 nuerons used. I used this as they were in the starter code to use. 

On the second, I added a third layer (AlphabetSoupCharity_Optimisation.ipynb), I set 37 neurons to be used on first, second and third layers. 

The last attempt, I set first hidden layer to use 156 neurons, second and third hidden layers with 39 neurons.

I noticed, when running the model more than once, it would create different result and accuracy.  
The activation function used for all hidden layers is relu, which is a common choice for deep learning models.
The output layer consists of a single neuron with a sigmoid activation function.


2. Were you able to achieve the target model performance?
No, despite ramdom and multiple attempts, I was not able to achieve the 75% model accuracy.
Maximum accuracy I could obtain was 73.516%

3. What steps did you take in your attempts to increase model performance?
I removed more columns, added more layers & added additional hidden nodes, and re-run the model of same layers in attempt to achieve higher model accuracy.

3. Summary: Summarise the overall results of the deep learning model. Include a recommendation for how a different model could solve this classi cation problem, and then explain your recommendation.
Overall, the deep learning model was around 73% accurate in predicting the classification problem. Using a model with greater correlation between input and output would likely result in higher prediction accuracy. This could be achieved by doing additional data cleanup up front, as well as by using a model with different activation functions and iterating until higher accuracy is reached.

The model does not achieve a target predictive of more than 75% accuracy, there could be due to the hidden nodes value used for the train model. 
Recommendation would the choice of best model and approach may require for further training of the model. 
