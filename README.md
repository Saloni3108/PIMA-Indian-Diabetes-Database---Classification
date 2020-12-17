# PIMA-Indian-Diabetes-Database---Classification
This repository contains Deep learning model using keras library for predicting the onset of diabetes based on diagnostic measures. The overfitting is reduced through Drop out and Regularization method.

1.	DESCRIPTION : Predict the onset of diabetes based on diagnostic measures.
2.	SUMMARY This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective is to predict based on diagnostic measurements whether a patient has diabetes.
Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.
Pregnancies: Number of times pregnant 
Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test 
BloodPressure: Diastolic blood pressure (mm Hg) 
SkinThickness: Triceps skin fold thickness (mm) 
Insulin: 2-Hour serum insulin (mu U/ml) 
BMI: Body mass index (weight in kg/(height in m)^2) 
DiabetesPedigreeFunction: Diabetes pedigree function 
Age: Age (years) 
Outcome: Class variable (0 or 1)

Overfiting
1.	Since our traning set has just 691 observations our model is more likely to get overfit, hence we have applied L2 -regulrization to the hidden layers.
2.	Weight Regularization is an approach to reduce the over-fitting of a deep learning neural network model on the training data and to improve the performance on the test data.
3.	Keras provides 3 kernel_regularizer instances (L1,L2,L1L2), they add a penalty for weight size to the loss function, thus reduces its predicting capability to some extent which in-turn helps prevent over-fit.


Use the Dropout regularization technique.

In this technique during the training process, randomly some selected neurons were ignored i.e ‘dropped-out’.
1.	Here we used 0.3 i.e we are dropping 30% of neurons randomly in a given layer during each iteration.
2.	We can set the different dropout percentage to each layer if required.
3.	Because of dropout, their contribution to the activation of downstream neurons is temporarily revoked and no weight updates are applied to those neurons during backward pass.


Regularization
1.	If neurons are randomly dropped during training, then the other neurons have to step in and handle the representation required to make the predictions for the missing neurons.
2.	This results in a better learning by all the neurons and hence network becomes less sensitive to the specific weights of neurons, so better generalization and less likely to overfit.

