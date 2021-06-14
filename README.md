
# Deep Learning Algorithms
This project uses different deep learning algorithms and all dataset are stored at Data folder. WE used Draw A Circel (DAC) and Touchalytics data.

## DAC:
* Draw A Circel (DAC) is a challenge-response based behavioral authentication system. It constructs a profile for each user, based on their circle drawing activity, and stores it at the server. During an authentication session, the collected user data is compared against stored profile to make an authentication decision. We use DAC data to train a Deep Neural Network. The number of vectors in each DAC profile is around 140-180 which is not suffeceint to train a Deep Neural Network. So, we first oversample the DAC data to increase the profile size. 


## Touchalytics:
* Touchalytics uses users' touch data (up-down and left-right scrolling) when interacting with an app. It uses the collected touch data for user authentication. The system uses 30 behavioral features and data from 41 users. We downloaded touchalytics data from the link http://www.mariofrank.net/touchalytics/. We then cleaned the data by replacing 'NaN' and 'Infinity' by zero and dropped the 'doc id', 'phone id', and 'change of finger orientation' columns. The number of vectors in each Touchalytics profile is around 300-1230. For some profile this data sample is not suffeceint to train a Deep Neural Network. So, we first oversample the Touchalytics data to increase the profile size. 

## Deep Neural Networks
* Neural Network Classifer (DAC): OversampledDACData.ipynb file has details about the data oversampling technique and implementation of a deep neural network classifer.
* Neural Network Classifer (Touchalytics): OversampledTouchalyticsOData.ipynb file has details about the data oversampling technique and implementation of a deep neural network classifer.
* AutoEncoder (Touchalytics): TouchalyticsAutoEncoder.ipynb file has details about the implementation of AutoEncoder.
