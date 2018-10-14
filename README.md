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
  - emoji count
  - textblob - polarity 
  - textblob - subjectivity
  - number of interjections
  - sarcastic word synonyms - need more clarity
  - pattern related feature - vector of words in the form of phrases - need to discuss more
  - write to file.
  
 classifier algorithm 
  - gradient boosting
  - random forest
  
 PART 2 : 
  neural network - to be discussed
