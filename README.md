# Disaster-Prediction-using-Adv-NLP

the goal of this notebook is to show several deep learning methods to solve the Disaster Tweets challenge. I'm going to start by presenting the data that we're going to study. Then I will present four deep learning models built using pytorch. To finally use these four models in a single prediction. The models will be created with pytorch.

## Indications before running the notebook.
You will only be able to run this notebook if you have a GPU, so if your computer does not have one you can go to Google Colaboratory to get access to a GPU. In the code below I assume that you have your notebook on google colaboratory and that you have modified the type of execution to activate a GPU. If so, you should see "Device: cuda" as a message.
Also I assume you have downloaded dataset locally. If this is the case you will need to modify path_data so that it indicates the position of the data.

### What should I expect the data format to be?
Each sample in the train and test set has the following information:

### The text of a tweet
A keyword from that tweet (although this may be blank!)
The location the tweet was sent from (may also be blank)
What am I predicting?
You are predicting whether a given tweet is about a real disaster or not. If so, predict a 1. If not, predict a 0.

#### Files
* train.csv - the training set
* test.csv - the test set
* sample_submission.csv - a sample submission file in the correct format
#### Columns
* id - a unique identifier for each tweet
* text - the text of the tweet
* location - the location the tweet was sent from (may be blank)
* keyword - a particular keyword from the tweet (may be blank)
* target - in train.csv only, this denotes whether a tweet is about a real disaster (1) or not (0)
