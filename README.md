# text-mining
COMP61332 Text Mining Coursework Report: Relation Extraction
This repository contains the implementations of a Hybrid BERT-Pair  

# Bert Pair 
This notebook contains the Bert-Pair approach to relation extraction. It should only be run after pretraining the model using the MTB_pretraining.ipynb file as we are trying to produce a hybrid model that is pretrained on MTB and then trained and evaluated on BERT-Pair.

The main goal is to gain understanding on different models and approached to relation extraction but also discover how much pretraining might or might not impact a model's performance in a different field. The pretrained model is also a part of the BERT family, more specifically BERT-MTB, and it is loaded as a checkpoint for a BERT-Pair model. The BERT-Pair model is then run using fewshot.

Given the size of our data sets and hardware limitations, we were greatly limited in running the model and fine tuning our parameters, especially the max_length, so we were only able to get to a threshold of 50% in most our runs because our model was not able to learn correctly. However, as we are not trying to beat the state-of-the-art approaches, we can still use our results to evaluate models and approaches, and find out if the pretraining has indeed impacted the results.