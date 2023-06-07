# Word2Vec_Gensim
I gonna use gensim to change whole phrases into vectors and do some operations on the text
# Link to the Dataset: http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Cell_Phones_and_Accessories_5.json.gz
# When i want to load a json dataset i need to specify "lines = True" it means that json objects will be sorted into lines
# I check shape, it is very big, I check first review 
# I gonna use "utils.simple_preprocess" from gensim to tokenize the first sentence
# Now i gonna do tokenization on every review in my dataset, so I apply above function, it gonna create lists with tokenized sentences
# Next I create gensim model and set parameters, first size of "window will be 10"  It means 10 before target word and 10 after target word
# Then "min count will be 2, so it gonna use sentence with min two words and last will be workers at 4, so it use four cpu's to work
# Now I specify vocabulary for my model on my "review_text" and it will show progress after every 1000 word
