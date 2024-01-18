Different types of predefined embeddings are:
a: Custom embeddings: We can do custom embeddings as well on our data but for that we need huge amount of data and we need to train our data as well which will take a lot of time.
b: Transformer based: Before encoder and decoder layer, we put the embedding layer to feed our model with numbers (vectors) and not with the text.
c: Word2Vec: Uses two approaches: Continuous bag-of-words (CBOW) and Skip-grams 
d: GLoVe (Global Vectors): extended version of Word2Vec in a n-dimensional space. Dot product of two things = log (likelihood of those two things appear together in a sentence) Eg: Tea, Coffee
e: FastText: extended version of Word2Vec but instead of skip-grams where we take a window size of and put words into that window, we take sub-words into the account. This works best when we havea unseen words in test data.
ELMo: Bi-directional LSTM and embedding depends upon the context of the word. Eg: 1: He was known to be fair; 2: The fair was so much fun. The word 'fun' has different context in both the sentences.
I tried different types of embedding using Gensim library like word2vec (wv), glove, fasttext. These are the predefined embeddings that can be used to find similarity between the words in the embedding space.
