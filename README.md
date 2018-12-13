# Sarcasm-Detection
project to predict sarcastic comment
 clean the dataset
 `- retain first 2 colunms i.e. sarcasticstatus and comment 
  - remove single word comments
  - remove words with #
  - remove non english comments
  - remove url and any other tagging
  - write data to a file.
  
 PART 1 : 
 
 create dictionary
  - emoticon dictionary
  - slang dictionary

 preprocess the data
  - replace the words within * * by capital letters and remove the * from comment 
  - map words of slang dictionary and replace with tokens
  - tokenization 
  - lametization
  - pos tagging 
  
 feature extraction
  - puntuation feature - count number of punctuation('!', '?', '.')
  - (!) is sarcastic
  - capitalization - (number of capital characters) - need more clarity
  - emoji count - Number of positive emoji and negative emoji
  - textblob - polarity 
  - textblob - subjectivity
  - number of interjections
  - pattern related feature - recognizing 3 patterns in a comment would lead to 3 million rows in a dataframe which is leading to memory                               error
  - Adding parent comment sentiment as a feature
  - write to file.
  
 classifier algorithm 
  - gradient boosting - Sirisha
  - random forest - Karuna
  - SVM - Nayana
  
  
  Accuracy - Check with unbalanced
  Accuracy - Check with more features
  -------------------------------------
  
  tokenization,pos tagging, num of interjections, - Nayana
  18,19,25,26 --- Sirisha 
  27,28,29,30 ---Karuna
  
 PART 2 : 
  Neural Network
  
  Prepare the dataset
    - Remove emoji's,hash tags, punctuations
    - Slang dictionary replacement - with and without
    - Convert the words to vector using word2vec or Glove 
    - Words not present in word2vec or glove are initialized randomly
    - One Hot Encoding - need to discuss
    
  Load the dataset
  Building the network
    - Num of layers to use - simple (2)
    - Activation functions - relu and sigmoid - good for classification tasks, softmax for last layer
    - Number of hidden neurons
  
  Compiling the network
    - Loss Functions - Binary Cross Entropy, Mean Squared Error
    - Optimizers - rmsprop,
    
  Train the model
    - Batch Sizes, Epoch (Num of iterations)
    
  Validate and calculate the accuracy
  
  
  Neural Network with parent comment - Nayana - try with all different iterations and functions
  Neural Network without parent comment - Karuna -  try with all different iterations and functions
  Neural n/w with slang dictionary replacement - Sirisha - without parent comment -  try with all different iterations and functions
  
  
  - Positive Word Count - Karuna
  - Negative Word Count - Karuna
  - Positive Intensifier - Karuna
  - Negative Intensifier - Karuna
  - Polarity Flip - Karuna
  
  
  Glove - Cosine - Embedding features - Nayana
  Word2Vec - Cosine - Embedding features - Sirisha
