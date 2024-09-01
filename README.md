CMPT 419 Final Project
Predicting Emotional OutBERSt

Danny Nguyen: dkn3@sfu.ca, 301449063
David Xiong: dxa14@sfu.ca, 301305081
Tegnoor Gill: tegnoorg@sfu.ca, 301344408

Code Structure and Navigation:
All code used google drive mounting for paths. To run the code locally, upload the audio files and csv files, and change the path to local paths.

The 'filtered_training_data.csv' are all the data used for training the models. The 'test_data.csv' is the data used for testing the model, and contains our inter-rated perceived emotions, as well as valence and arousal. It is a 100 subset taken from the original training data (i.e. filtered_training_data = training_data - 100 used for test_data).

Self Evaluation/Reflection: 
In our proposal, we wanted to test the BERSt audio data on 3 different models; CNN, RNN, and CRNN. At the time, we did not decide which method of feature extraction to use. After doing research, we decided on extracting the MFCCs. 
We were able to achieve our goal of training and testing on 3 models, and find the best performing models. We were also able to label our perceived emotion on 100 selected files. Our results quantified the each models performance with an F1 score and an accuracy rating. 

However, we were only able to test the models on the extracted MFCCs of the training data. Despite our efforts, we did not have the expertise to train the models on MFCCs as well as other features including 'first_language', 'gender', and 'prompt'. For future improvements, we would like to train the model with the aforementioned features alongside the MFCC features, in hopes it would yield a more interesting result. 
