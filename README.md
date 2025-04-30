# deep-learning-challenge
Deploying Machine Learning
Author: Jeff Gielniak
Date: 2025-04-29

Data Processing:
This code imports information from a CSV that has data on venture funding of over 34,000 organizations.  Using the CSV, I cleaned, preprocessed, and scaled the data to prepare it for entry into the model.  I used the 'IS SUCCESSFUL' column as the target for my model, and the remaining data (organization, ask amount, income amount, etc) were all used as features of the model.  The name and identification numbers were removed before the processing since they had no value as input data.  The goal for the model was to predict if a given campaign was successful based off the other data in the dataframe (the features).

Compiling, Training and Evaluating:
At that point, I designed a Neural Network model to train and test with the dataset.  I used TensorFlow and Keras to define dense layers, and then ran the model for 100 Epochs.  The two hidden dense layers used 80 and 30 units respectively. I then used the test data to calculate the loss and accuracy, followed by exporting the model to an HDF5 file. 
![image](https://github.com/user-attachments/assets/927fde3c-ebcd-42e7-b995-62dce82a0de8)
Results
The model did not perform very well, with an accuracy of only about 73% and a loss of over 0.5.  I attempted to add an additional dense layer to improve accuracy, but that did not help.  
![image](https://github.com/user-attachments/assets/6972dea6-8157-4fb7-a9ad-06df28ffff33)
