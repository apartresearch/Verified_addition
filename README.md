# Official Repository for Increasing Trust in Language Models through the Reuse of Verified Circuits 
### Authors Philip Quirke, Clement Neo and Fazl Barez

Understanding the inner workings of machine learning models like Transformers is vital for their safe and ethical use. 
This repository contains Colabs that train addition models, subtraction models, addition and subtraction models.
The resulting models have very low loss and can correctly predict one million succcessive questions.  

The associated [paper](https://arxiv.org/abs/2402.02619) details the algorithm of the addition algorithm:

<img src="https://github.com/apartresearch/verified_addition/blob/main/figures/addition_2_jpg.001.jpeg" width="600">

The [Accurate_Math_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Math_Train.ipynb) supports the optional re-use of one model when training a new model:

<img src="https://github.com/apartresearch/verified_addition/blob/main/figures/addition_jpg.001.jpeg" width="600">

Our initial (less capable) Colabs:
- train a perfectly accurate 5-digit integer addition model ( [Accurate_Addition_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Addition_Train.ipynb) ) and
- analyse the trained model to reveal its algorithm, and using intervention ablation and Principal Component Analysis to verify the algorithm ( [Accurate_Addition_Analyse.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Addition_Analyse.ipynb) )

Our final (more-advanced) Colabs:
- train a n-digit integer addition model, or subtraction model, or "addition and subtraction" model ( [Accurate_Math_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Math_Train.ipynb) )
- allow the untrained "addition and subtraction" model to be initialised with a trained "addition" model as an experiment in model re-use 
- analyse the trained models using to provide insights into their algorithms  ( [Accurate_Math_Analyse.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Math_Analyse.ipynb) )

The [Accurate_Math_Train.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Math_Train.ipynb) Colab is preconfigured to train 9 different models (with 5 or 6 digits, 2 or 3 layers, 3 or 4 heads, doing addition, subtraction or both). A one-line code change in "Part 1B" swaps between these models. Training of one model can take ~30 minutes. The trained model weights (*.pth) are saved to a public [HuggingFace](https://huggingface.co/PhilipQuirke/Accurate6DigitSubtraction/tree/main) folder.

The [Accurate_Math_Analyse.ipynb](https://github.com/apartresearch/verified_addition/blob/main/assets/Accurate_Math_Analyse.ipynb) Colab is preconfigured to analyse 7 different models (with 5 or 6 digits, 2 or 3 layers, 3 or 4 heads, doing addition, subtraction or both). A one-line code change in "Part 1B" swaps between these models. For speed, this CoLab loads the selected model weights from the public [HuggingFace](https://huggingface.co/PhilipQuirke/Accurate6DigitSubtraction/tree/main) folder, allowing the analysis to start promptly. The Colab produces various graphs displaying its analysis.


### Reference

If you use our work, please consider citing:

```
@misc{quirke2024increasing,
      title={Increasing Trust in Language Models through the Reuse of Verified Circuits}, 
      author={Philip Quirke and Clement Neo and Fazl Barez},
      year={2024},
      eprint={2402.02619},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}

