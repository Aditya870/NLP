Classification Of Diabetic Patient Using Keras

Dataset:

You have to use “Pima Indians Diabetes Dataset” for this task. The dataset can be downloaded from the kaggle website which can be found in below link

https://https://drive.google.com/file/d/1gb7ViqiTQuhNeB_iYvpEs_o6czwri4Oi/view?usp=sharing

Dataset Description:

Description of variables in the dataset:

  • Pregnancies: Number of times pregnant.
  
  • Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.
  
  • Blood Pressure: Diastolic blood pressure (mm Hg).
  
  • Skin Thickness: Triceps skin fold thickness (mm).
  
  • Insulin: 2-Hour serum insulin (mu U/ml).
  
  • BMI: Body mass index (weight in kg/(height in m)²).
  
  • Diabetes Pedigree Function: Diabetes pedigree function.
  
  • Age: Age (years).
  
  • Outcome: Class variable (0 or 1).

Implementation steps :

• Visualise the data using multiple types of plot function. 

• Split data into Training and Testing sets. Test set should contain 25 % of the original data. 

• NN should contain two hidden layers. Both the hidden layers use “sigmoid activation function”. Number
of hidden units in first and second hidden layers are 512 and 128 respectively. The output layer uses
softmax activation functions. Batch size is 32 and number of epochs are set to 1000. Take initial learning
rate as 0.005.

• Print the accuracy and classification report.

• Report the accuracy (test set) on Batch size is 16 and Batch size is 48. 

• Also, Report the accuracy (test set) on different learning rate such as 0.01 and 0.001.

