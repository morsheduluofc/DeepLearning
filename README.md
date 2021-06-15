
# Deep Learning Algorithms
This project uses different deep learning algorithms on the data set of two behavioral authentication systems: Draw A Circel (DAC) and Touchalytics. All dataset are stored at the 'Data' folder.

## DAC:
* Draw A Circel (DAC) is a challenge-response based behavioral authentication system. It constructs the profile for each user based on their circle drawing activities in an app, and stores it at the server. During the authentication session, the new collected data is compared against the stored profile to make an authentication decision. The number of vectors in each DAC profile are around 140-180 and they are not suffeceint to train a Deep Neural Network. So, we first oversampled the DAC data to increase the number of vector in each profile. 


## Touchalytics:
* Touchalytics uses users' touch data (up-down and left-right scrolling) when interacting with an app. It uses the collected touch data for user authentication. The authentication system uses 30 behavioral features and data from 41 users. We downloaded touchalytics data from the link http://www.mariofrank.net/touchalytics/ and cleaned it by replacing 'NaN' and 'Infinity' by zero, and dropped the 'doc id', 'phone id', and 'change of finger orientation' columns. The number of vectors in each Touchalytics profile is around 300-1230. For some profiles this data sample (vector) are not suffeceint to train a Deep Neural Network. So, we first oversampled the Touchalytics data to increase the number of vector in each profile.

## Neural Network Algorihms:
* Neural Network Classifer: 
  * DAC classifier: OversampledDACData.ipynb file has details about DAC data oversampling technique. It then construct a deep neural network classifer and used the oversampled data to train it.
  * Touchalytics classifer: OversampledTouchalyticsOData.ipynb file has details about Touchalytics data oversampling technique. It then construct a deep neural network classifer and used the oversampled data to train it.
* AutoEncoder 
  * Touchalytics AutoEncoder: TouchalyticsAutoEncoder.ipynb file has details about the implementation of Touchalytics AutoEncoder.
