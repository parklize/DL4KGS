# DL4KGS
This page provides the details of domain-specific embeddings learned from different aspects of DBpedia for the following submission.

## Node2Vec
The vectors are [gensim](https://radimrehurek.com/gensim/) KeyedVectors, therefore, it can be loaded using KeyedVectors.
```
ent_vectors = KeyedVectors.load_word2vec_format('tmp/'+domain+'/walks.txt.gz', binary=True)
```
For example, the vector for "entityName" can be accessed by ent_vectors['http://dbpedia.org/resource/entityName'], and please refer to https://radimrehurek.com/gensim/models/keyedvectors.html for more functions.
- [book](https://drive.google.com/open?id=1E3FscznHFfFbqtk9ydaRbdAFG80R7SuB)
- [music](https://drive.google.com/open?id=17rvBNN1tpPG_JhlFGEN_jRH816fz6JMm)

## TransE
- [book]
- [music](https://drive.google.com/open?id=1ZzFRyESVLslsCeGxq_gPaNdnOjALRx7Y)

