# Sentiment-Analysis-of-Memes

To perform sentiment analysis on memes and classify the type of emotion that they depict using Logistic Regression, Naive Bayes, Feed Forward Neural Network,
Convolutional Neural Network and BERT. 

This project is based on the Memotion Analysis problem in SemEval-2019 Task 8 https://competitions.codalab.org/competitions/20629#learn_the_details-overview 


"data" folder contains the csv files: 

  labels.csv - train dataset downloaded from https://www.kaggle.com/williamscott701/memotion-dataset-7k 
  2000_testdata.csv - test dataset downloaded from https://competitions.codalab.org/competitions/20629#learn_the_details-overview 
  Test_Actual_Final.csv - contains the ground truth value of the emotions - used in testing for calculating accuracy

"code" folder contains the notebook files
Steps to run the code:

1) Please create a folder in google drive /NLP_Project/ and place here the csv files provided under the folder "data".

(Ideally the path for files will be /content/gdrive/Mydrive/NLP_Project/)

2) Files should run in the following order sequentially one after another(because of dependencies) 

1. LR_NB (takes as input labels.csv file and 2000_test_data.csv)
2. followed by FFNN
3. then CNN
4. then Sampling
5. then BERT

(The codes generates other csv files with corresponding output while running, which will be used further)




