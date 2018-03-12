# DL4KGS
This page provides the details of domain-specific embeddings learned from different aspects of DBpedia for the following submission.

## Node2Vec
The vectors are [gensim](https://radimrehurek.com/gensim/) KeyedVectors, therefore, it can be loaded using KeyedVectors.
```
ent_vectors = KeyedVectors.load_word2vec_format('tmp/'+domain+'/walks.txt.gz', binary=True)
sim = ent_vectors.similarity(item, c)
```
For example, the vector for "entityName" can be accessed by ent_vectors['http://dbpedia.org/resource/entityName'], and please refer to https://radimrehurek.com/gensim/models/keyedvectors.html for more functions.
- [book](https://drive.google.com/open?id=1E3FscznHFfFbqtk9ydaRbdAFG80R7SuB)
- [music](https://drive.google.com/open?id=17rvBNN1tpPG_JhlFGEN_jRH816fz6JMm)

## TransE
The provided files consist of (1) item/entity indices & (2) corresponding vectors.
- [book](https://drive.google.com/open?id=1pRlU3R-u2lgBEhX7dDA5lgDu9uWDKijS)
- [music](https://drive.google.com/open?id=1ZzFRyESVLslsCeGxq_gPaNdnOjALRx7Y)

## Doc2Vec
The vectors are gensim Doc2Vec model, a simple example of measuring similarity between two URIs (item, c) is as below:
```
model = Doc2Vec.load(path)
sim = model.docvecs.similarity(item, c)
```
- [book](https://drive.google.com/open?id=1gfAYN-RDnxnyFAHHnfP2s8l7_avqhWmO)
- [music](https://drive.google.com/open?id=10DNLzGg6qH-GCfAMI4-rWc45QbpYie1i)
