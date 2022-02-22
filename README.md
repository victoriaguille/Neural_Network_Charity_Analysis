# Neural_Network_Charity_Analysis
### Overview
####
A foundation, Alphabet Soup, that helps fund nonprofits and charities through large donations has noticed an uptick in certain groups taking the funding and not succeeding in the initial goals described to the foundation. The foundation has requested that an analysis be performed using neural networks to predict if a charity will succeed with funding. Using a CSV file that contains data on previous charities that were given donations from the foundation, Python, and Colab, an analysis was performed to see if a reliable prediction of success could be made. 

### Results
####
Below are the findings from the preprocessing portion of the analysis. 
 - The target of the model is whether or not a charity was successful in their goals with funding. The particular column this information would be found under is the "IS_SUCCESSFUL" column. 
 - The features of the model are the remaining columns once the "IS_SUCCESSFUL", "EIN", and "NAME" columns are removed from the dataframe. 
####
![xandy](link)
####
 - Only two columns held variables that were neither targets nor features, the "EIN" and "NAME" columns which were promptly dropped from the input data before any real preprocessing began. 
####
![einandname](link)

####
Below are the findings from the compiling, training, and evaluating of the model. 
- For the first neural network model, the length of the X_train were the amount of neurons selected for the feature, there were two hidden layers, and activation functions used were the relu and sigmoid functions. This was a great first approach to the model choice. 
####
![firstmodel](link)
####
- The target model performance of 75% or higher was not achieved, regardless of attempts to optimize. The highest the accuracy rating got was 73%.
####
![highestaccuracy](link)
####
- Three attempts were made to optimize the neural network model with little success. With each new model, the size and number of hidden layers grew along with a shift of using the relu activation to the tahn activation function to achieve the best accuracy percentage. 
####
![finalmodel](link)

### Summary
####
The acceptable rate of success for the neural network model that was performed for this analysis was 75%, however, none of the models reached that accuracy goal. Due to this, none of the models could be used to properly predict whether a charity would succeed with funding from Alphabet Soup. Each attempt at optimization increased the number of hidden layers and epochs, but there was little change in the loss and accuracy of the individual models. A different approach would need to be utilized in order to achieve the acceptable range of accuracy. A future data analyst may find success in employing the keras tuner method as it will perform several models to find the best fit for the data behind the scenes.  
