
# Deep Learning Algorithms
This project uses different deep learning algorithms and all dataset are stored at Data folder.

## Deep Neural Network Classifer for DAC:
* Draw A Circel (DAC) is a challenge-response based behavioral authentication system. It constructs a profile for each user, based on their circle drawing activity, and stores it at the server. During an authentication session, the collected user data is compared against stored profile to make an authentication decision. We use DAC data to train a Deep Neural Network Classifer. The number of vectors in each DAC profile is around 140-180 which is not suffeceint to train a Deep Neural Network. So, we first oversample the DAC data to increase the profile size. OversampledDACData.ipynb file has details about the implementation.


## Deep Neural Network Classifer for Touchalytics:
* ssifier.ipynb file
