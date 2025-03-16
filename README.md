Enhancing Mixed Oil Length through Graph Representation Learning
===============================================================================

About
-----
This repository is the official PyTorch implementation of "Enhancing Mixed Oil Length through Graph Representation Learning". 

We propose a new model based on graph representation learning to predict mixed oil length. Specifically, our method explicitly models the dependencies among mixed oil samples using a graph representation learning framework, thereby overcoming the limitation of previous methods that assume sample independence. This repository includes how to train our model and how to predict using our model.

Installation
------------
At the root folder:
```bash
conda env create -f environment.yml
conda activate grape
```

Install [PyTorch](https://pytorch.org/)

Install [PyTorch_Geometric](https://rusty1s.github.io/pytorch_geometric/build/html/notes/installation.html)

Usages
------

To train the model and predict mixed oil on oil datasets:

Step1: Put data into "oil/raw_data/oil/data/data.txt". You can change the index of training features and target feature based on your oil data in "oil/raw_data/oil/data/index_features.txt" and "oil/raw_data/oil/data/index_target.txt".

Step2: Run "mixed_oil_length_prediction.py".

Step3: The training model will be saved in "oil/test/result.pkl". The figure will be saved in "oil/test/curve.png". The prediction results will be saved in "pred_test.txt".
