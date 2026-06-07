Scenario
You are tasked with solving an image classification problem. One approach is to extract features from images (such as color histograms, texture features, or 
embeddings from a pretrained CNN) and train an XGBoost model. Another approach is to train or fine-tune a deep learning model such as ResNet or EfficientNet.

Question
Suppose you are tasked with solving an image classification problem. One option is to extract features from images 
(e.g., color histograms, texture features, or embeddings from a pretrained CNN) and train an XGBoost model. 
Another option is to train or fine-tune a deep learning model (like ResNet or EfficientNet). Discuss the two approaches.



what is the funcdemental differnce between how convolution neural networks differ from xg boost in image data.??


how does trnsfer learnign and cnns bridge the gap of compute and small data sets




how does the qualty of features extracted in XG boost compare with what CNN is learning from raw images

Learn more about xg boost vs this comparison
Understand in detail about xgboost in image classfriciation
Manually extracted features 
feature learning and representation
CNN and XG Boost?

timestamps and created information integrating into the CNN vs XG boost




Problem Description
Scenario
You are improving the training stability and performance of a very deep convolutional neural network (CNN) for a challenging image classification task. 
During training, you observe issues such as vanishing/exploding gradients and slow convergence.

Question
You are improving the training stability and performance of a deep CNN for a challenging image classification problem. 
The network is very deep, and you notice issues with vanishing/exploding gradients and slow convergence. 

How would techniques such as batch normalization, residual connections (as in ResNets), and careful weight initialization help address these problems?


3 things and vanishing gradient problem

any other techniques to mitigate vanishing gradient 


In convolutional neural networks (CNNs), convolutional filters and pooling layers play a critical role in extracting meaningful features from input data while reducing spatial dimensions and computational complexity.

Question
In convolutional neural networks (CNNs), filters and pooling layers play critical roles in feature extraction and dimensionality reduction. 
How would you explain the roles of different types of pooling (max, average, min) and convolutional filters, and when each might be useful?



Max pooling vs average pooling when do you prefer each one ?

how would you design a number of filters and layers when desigining a new CNN?

how does padding effect output of colvolutions and edges when preservving features around edges


why do deeper cnns capture more abstract features than earlier layers


An advertising agency wants to forecast weekly ad impressions for its online campaigns. 
The data shows clear seasonal patterns (e.g., higher traffic on weekends and holidays) and also
includes external variables such as marketing budget, competitor ad spend, and major events.

Question
How would you use a SARIMAX model to build a robust forecasting solution?


Seasonality
AUto Regressive
Moveing Averaa


pde 
ARIMA how would you calcualte the values 

ADF Test (Augmented Dickey-Fuller)

PACF = Partial AutoCorrelation Function

ACF = AutoCorrelation Function

how do you add exoginours variables 

how do you handle missing values if there is any in SARIMAX

what assumptions about seasonanility and stationarityb would we consider before fittig a SRIMAX data

statinality and repeated seasonal 

You are working on a sequence modeling problem where understanding how information flows over time is critical. Earlier approaches relied on Recurrent Neural Networks (RNNs), but Long Short-Term Memory (LSTM) networks were introduced to address their limitations.

Question
Recurrent Neural Networks (RNNs) were once the standard for sequence modeling tasks, but Long Short-Term Memory networks (LSTMs) improved on their limitations.
Compare RNNs and LSTMs in terms of their architecture, ability to capture long-term dependencies, and practical performance on sequence tasks.



Bi directional RNNS and LSTMS

GRR alternative to LSTMS?

Problem Description
Question
You are implementing your own version of TF IDF (Term Frequency Inverse Document Frequency) for a small corpus of text reviews. You are given a Pandas DataFrame with a column "review" containing text data.

You need to:

Tokenize each review (split by spaces)
Compute Term Frequency (TF) for each document
Compute Inverse Document Frequency (IDF) for all unique words
Combine them to form a TF IDF matrix as a Pandas DataFrame
Rows = documents
Columns = unique words
Constraint: You may only use NumPy, Pandas, and built in Python libraries (no sklearn, nltk, etc.).

Problem Description
Question
You are implementing your own version of TF IDF (Term Frequency Inverse Document Frequency) for a small corpus of text reviews. You are given a Pandas DataFrame with a column "review" containing text data.

You need to:

Tokenize each review (split by spaces)
Compute Term Frequency (TF) for each document
Compute Inverse Document Frequency (IDF) for all unique words
Combine them to form a TF IDF matrix as a Pandas DataFrame
Rows = documents
Columns = unique words
Constraint: You may only use NumPy, Pandas, and built in Python libraries (no sklearn, nltk, etc.).


