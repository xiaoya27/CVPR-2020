# CVPR-2020
Valuable notes and toy projects from CVPR 2020 Tutorial on Image Retrieval in the Wild

## this is a summary of [CVPR 2020 Tutorial on Image Retrieval](https://matsui528.github.io/cvpr2020_tutorial_retrieval/) in the Wild, I have found Matsui Sensei's talk on Billion scale Approximate Nearest Neighbor Search extremely informative, therefore I tried to summarize  the key points in here for my own reference.


![img](/imgs/cheatsheet.PNG)


### Research Question: Given a query 𝒒, find the closest vector from the database(One of the fundamental problems in computer science)

#### Solution: 
1. Nearest Neighbor Search(NN) :worried:

    linear scan, 𝑂(𝑁𝐷), slow 

2. Approximate Nearest Neighbor Search(ANN) :blush:

    Faster search
    Don’t necessarily have to be exact neighbors
    Trade off: runtime, accuracy, and memory consumption

#### Solution Implementation 
##### NN
Naïve implementation

Fast implementation (by Faiss) : Matrix multiplication by BLAS

ps : NN in GPU (faiss gpu ) is 10x faster than NN in CPU faiss cpu

##### ANN
![img](/imgs/alg.PNG)
