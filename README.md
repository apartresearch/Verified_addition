## Official Repository for Increasing Trust in Language Models through the Reuse of Verified Circuits | Authors Philip Quirke, Clement Neo and Fazl Barez

Understanding the inner workings of machine learning models like Transformers is vital for their safe and ethical use. 
This repository contains Colabs that train addition models, subtraction models, addition and subtraction models, with optional re-use of one model when training another.
The resulting models have very low loss and can correctly predict one million succcessive questions.  

This repository contains our initial Colabs that:
- train a perfectly accurate 5-digit integer addition model ( [./Accurate_Addition_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/Accurate_Addition_Train.ipynb) ) and
- analyse the trained model to reveal its algorithm, and using intervention ablation and Principal Component Analysis to verify the algorithm ( [./Accurate_Addition_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/Accurate_Addition_Analyse.ipynb) )
 
The associated [paper](https://arxiv.org/abs/2402.02619) summarises the results of these Colabs 

This repository also contains more-advanced Colabs that:
- train a n-digit integer addition model, or subtraction model, or "addition and subtraction" model ( [./Accurate_Math_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/Accurate_Math_Train.ipynb) )
- allow the untrained "addition and subtraction" model to be initialised with a trained "addition" model as an experiment in model re-use 
- analyse the trained models using to provide insights into their algorithms  ( [./Accurate_Addition_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/Accurate_Math_Analyse.ipynb) )

The same [paper](https://arxiv.org/abs/2402.02619) also summarises the results of these Colabs 
