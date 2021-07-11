# neural_network_charity_analysis

## Purpose:
The purpose of this analysis is to identify which applying companies will be ideal for Alphabet Soup to invest in. Input data has been collected from Alphabet Soups prior investment companies. 

## Restults:

### Data Preprocessing
- The target or outcome variable for this model is the success of the company that has been invested in. In this data set, the variable is known as "IS_SUCCESSFUL".
- The feature variables of this model, or the variables that will be input to train the model and predict whether future companies have a high probaility of success are: STATUS, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. 
- Variables that were removed at the onset of model formation due to a lack of relevance were the NAME and EIN.
- In future models, ASK_AMT was binned as well to help simplify the data with improvement in accuracy noted, but not more than the target 75%. 

### Compiling, Trainging, & Model Evaluation 
-Initial model desin includes 80 neurons in hidden layer 1 and 30 neurons in hidden layer two with both hidden layers being 'relu' activation types. Relu was chosen due to the non-linear aspect of the data set and the stength that relu has with regression modeling. The output layer is a single output with sigmoid activation.  
-In future models, a third hidden layer cantaining 10 more neurons was created, also designated as relu activation. The number of epochs was also increased 
-Modification of the data set and neural network model did show improvment to the accuracy of predictions from this model, but 75% accuracy was still not attained. 

## Summary
In this instance, neural network modeling could be viable in provding accurate predicitons if further parameters are modified, such as changing the optimizer or modifying the input data further, however simpler models may prove to work better. Models such as Random Forests, SVM and even more simple models like Logistic Regression have been shown in certain cases to be as effective as neural networks and may actually provide better accuracy by reducing the complication level of models processing to reduce noise in the data and a more direct calculation. As the data was processed more and more, it appeared that accuracy declined, so perhaps a simpler model would provide better accuracy. 

## Figures

### Initial model outcomes:
![Initial](https://github.com/ghynox/neural_network_charity_analysis/blob/main/NN_output_v1.png)

### Binning ASK_AMT
![ASK binned](https://github.com/ghynox/neural_network_charity_analysis/blob/main/NN_output_AMTbinned1.png)

### Increasing Hidden Layers
![3Layers](https://github.com/ghynox/neural_network_charity_analysis/blob/main/NN_output_3layers1.png)

### Increasing Epochs
![100Epochs](https://github.com/ghynox/neural_network_charity_analysis/blob/main/NN_output_100epoch1.png)
