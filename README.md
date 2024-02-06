## Official Repository for Increasing Trust in Language Models through the Reuse of Verified Circuits | Authors Philip Quirke and Clement Neo and Fazl Barez


Understanding the inner workings of machine learning models like Transformers is vital for their safe and ethical use. 
This repository contains a CoLab ( [./Accurate_Addition_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/Accurate_Addition_Train.ipynb.ipynb) ) that presents an in-depth analysis of a two-layer Transformer model trained for integer addition.

The CoLab creates, trains and then analyses a 2 layer Transformer model that performs integer addition e.g. 33357+82243=115600. Each digit is a separate token. For 5 digit addition, the model is given 12 "question" (input) tokens, and the model must then predict the correct 6 "answer" (output) tokens  
