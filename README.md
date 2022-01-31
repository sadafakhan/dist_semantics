## Description

Program that creates and evaluates a distributional model of word similarity based on local context term cooccurrence. Reads in a corpus that forms the basis of the distributional model and performs basic preprocessing. 

For each the word in the corpus, creates a vector representation based on word cooccurrence in a specified window around the word. Each element in the vector is weighted according to the input parameter (point-wise mutual information e.g. PMI and term frequency e.g. FREQ).

Reads in a file of human judgements of word-pair similarity and for each word in the pair, outputs to a file the word and its 10 highest weighted features and their weights. Computes the similarity between the two words based on cosine similarity and the spearman correlation between the similarity scores. 