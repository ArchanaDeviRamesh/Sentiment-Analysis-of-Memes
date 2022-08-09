# Sentiment-Analysis-of-Memes

* To perform sentiment analysis on memes and classify the type of emotion that they depict using Naive Bayes(NB) and Logistic Regression(LR), neural network models namely Feed Forward Neural Network (FFNN) and Convolutional Neural Network (CNN), and a transformer based model namely Bidirectional Encoder Representations from Transformers (BERT). This work also tests the system by handling the class imbalance issue which was not dealt in the competition

* This project is inspired by one of competition on the Memotion Analysis problem in SemEval-2019 Task 8 https://competitions.codalab.org/competitions/20629#learn_the_details-overview 

# Problem Definition

* Given an Internet meme, the first task which is a multi class classification problem classifies the meme’s sentiment as positive, negative or neutral and the second task which is a multi label classification problem classifies the type of emotion expressed as sarcastic, humorous, offensive or motivation meme.
For example, consider the meme given in following figure. The proposed system will classify the sentiment of this meme as positive and humour as motivational.

![img1](https://user-images.githubusercontent.com/105897803/182281147-2f1182e1-2ceb-4870-a789-2de8f221b134.png)

* Libraries used: pandas, numpy, matplotlib, sklearn, nltk, gensim, torch, tensorflow, transformers

# Repository folders

* "data" folder contains the following csv files: 

  -- labels.csv - train dataset downloaded from https://www.kaggle.com/williamscott701/memotion-dataset-7k 
  
  -- 2000_testdata.csv - test dataset downloaded from https://competitions.codalab.org/competitions/20629#learn_the_details-overview 
  
  -- Test_Actual_Final.csv - contains the ground truth value of the emotions - used in testing for calculating accuracy

* "code" folder contains the notebook files required 

# Steps to run the code

* Please create a folder in google drive /NLP_Project/ and place here the csv files provided under the folder "data".

    (Ideally the path for files will be /content/gdrive/Mydrive/NLP_Project/)

* Files should be run in the following order sequentially one after another(because of dependencies) 

      1) LR_NB (takes as input labels.csv file and 2000_test_data.csv)
      2) followed by FFNN
      3) then CNN
      4) then Sampling
      5) then BERT

    (The codes generates other csv files with corresponding output while running, which will be used further)


# Results:

CNN outperformed both the tasks compared to the baseline results considering Macro F1 as the criteria for evaluating performance.


