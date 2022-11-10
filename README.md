# Deep-Learning
deep-learning-challenge
Report on the Neural Network Model
#Deep Learning using hyper-tuned Neural Networks.
Overview:
EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively
EIN                       34299
NAME                      19568
APPLICATION_TYPE             17
AFFILIATION                   6
CLASSIFICATION               71
USE_CASE                      5
ORGANIZATION                  4
STATUS                        2
INCOME_AMT                    9
SPECIAL_CONSIDERATIONS        2
ASK_AMT                    8747
IS_SUCCESSFUL                 2
dtype: int64

##**Summary:**
The final automatically optimized neural network trained model from the keras tuner method achieved 73% prediction accuracy with a 0.55 loss, using a sigmoid activation function with input node of 76 neurons split and 50 training epochs. Performing better than the non automized model. Keeping the Name column was crucial in achieving and and going beyond the target. 

##**The losses were at 56% and accuracy was at 73%**
model_loss, model_accuracy = nn.evaluate(X_test_scaled, y_test, verbose=2)
print(f'Model Loss: {model_loss}, Model Accuracy: {model_accuracy}')
8575/8575 - 0s - **loss: 0.5578 - acc: 0.7263**
**Loss: 0.557812534073699, Accuracy: 0.7262973785400391**
