# Overview
The purpose of this analysis was to create a binary classifier that is capable of predicting whether loan applicants will be successful if funded.

# Results
  * Data Preprocessing
      * What variable(s) are considered the target(s) for your model? 
        * The IS_SUCCESSFUL variable was my target.
      * What variable(s) are considered to be the features for your model? 
        * Features of the model include Application Type, Affiliation, Classification, Use_Case, Organization, Income Amt, and Special Considerations. 
      * What variable(s) are neither targets nor features, and should be removed from the input data? 
        * I removed EIN, Name, and originally, Status. Reviewing the data, I would go back and remove Organization, Special Considerations, and potentially Use case.
  
  * Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why? 
      * I initially selected 2 hidden layers, with 80 and 50 neurons, respectively. Activation function was 'relu', and the single output layer had a 'sigmoid' activation function. I made these selections based on my understanding of how neural networks work, and knowing that deep neural networks require more than one hidden layer.
    * Were you able to achieve the target model performance? 
      * I was NOT able to achieve the target model performance of 75% accuracy. 
    * What steps did you take to try and increase model performance? 
      * I attempted to reduce bins of data, adjusted number of epochs, and added an additional layer with 10 neurons with 'relu' activation. I also attempted increasing data bins, increasing epochs, and keeping the additional layer. My last attempt included using Keras Tuning and applying Hyperparameters.
  
# Summary
All of the models I produced failed to achieve the target model performance of 75%. The closest my model achieved was 72.4% accuracy. The lowest accuracy achieved was 70%. The time spent attempting optimization might have been better suited gaining a deeper understanding of what the various activation functions do. The singular performance threshold would have been better informed by some additional preprocessing and cleaning of the data. I think that further breaking down some of the data bins (e.g., application types were skewed significantly to T3, and classification also significantly skewed to C1000) might yield improved accuracy.
      
