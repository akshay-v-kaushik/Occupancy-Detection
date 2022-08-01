# Occupancy Detection
Occupancy of an office room prediction 

### Introduction:-

Previous studies showed that knowing occupancy certainly can save energy in the control system of building. Here, Ground-truth occupancy is obtained from time-stamped pictures of environmental variables like temperature, humidity, light, CO2 were taken every minute. The implementation of an ML algorithm instead of a physical PIR sensor will be cost and maintenance-free.  In this regard, occupancy detection has a significant role in many smart building applications such as heating, cooling,
ventilation (HVAC) and lighting system.

### About the dataset:-

The data set can be loaded from the following link: https://archive.ics.uci.edu/ml/datasets/Occupancy+Detection+
It is a zip file consisting of three data sets that were used in the evaluation of the accuracy of predicting the occupancy of the room- one for training, and two for testing the models considering the office door opened and closed during occupancy. 
The attributes in the datasets are-
1. date on which the following physical parameters where observed and recorded
2. Temperature of the room in Celsius
3.Relative Humidity in %
4. Light in Lux
5. CO2 in ppm
6. Humidity Ratio derived quantity from temperature and relative humidity, in kgwater-vapor/kg-air and 
7. Occupancy- 0 or 1, 0 for not occupied, 1 for occupied status.
Occupancy is the target value to be used for prediction.

### Results that were obtained with this project:- 
I've trained the model using Neural networks and Logistic regression, written as raw codes, once with just one variable and again with two variables.
It was observed that Neural networks gave an accuracy of 98.84% and Logistic regression gave an accuracy of 98.64%. 
Both the algorithms gave pretty good accuracies. 
* Accuracies with Neural Networks
    * Training data with test data 1
    
     | Training accuracy  | Validation accuracy |
     | -----------------  | ------------------- |
     |     98.84%         |     97.07%          |
    * Training data with test data 2
    
     |   Training accuracy  | Validation accuracy |
     |   -----------------  | ------------------- |
     |       98.84%         |    91.97%           | 
            
* Accuracies with Logistic Regression
    * With one variable 
    
    |  Training accuracy  | Test accuracy 1 | Test accuracy 2 |
    |  -----------------  | --------------- | --------------- |
    |         97.87%      |      97.86%     |   99.14%        |
    
    * With two variables 
    
    |  Training accuracy  | Test accuracy 1 | Test accuracy 2 |
    | --------------      | --------------- | --------------- |
    |         98.64%      |      97.89%     |   82.48%        | 
    
Let's dive in and see how this was achieved.

I've written the code in google colab. You can download the files and work on it if you'd like.
1. View the file in the following order:
    1. [Occupancy-Visualization](https://colab.research.google.com/drive/1QbQwK3mvy4LVsgF87AaAmxYqvkYjrsRw)
    2. [Occupancy detection - Neural networks](https://colab.research.google.com/drive/1MHOY4Ocnzs-LipzXajYKV2h0mb-0ZG9c#scrollTo=c0xKW3Na54n7)
    3. [Occupancy detection -Logistic Regression for one variable](https://colab.research.google.com/drive/1s4o7bCubEHCQv97jzcCl9gm5vHl-_5aI#scrollTo=cSfpK3BrUqtY)
    4. [Occupancy detection -Logistic Regression for two variables](https://colab.research.google.com/drive/1aUQz2Cbd9YTtWJUrGywWt6SfpoTvo80J#scrollTo=ZKYGlvk3TvdN)
 2. You can download the files after viewing them and work on it if you'd like.

