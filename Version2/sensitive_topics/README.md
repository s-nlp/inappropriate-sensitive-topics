## Sensitive topics dataset

The sensitive topics dataset contains Russian sentences labelled for the presence of sensitive topics. The data files contain the following columns:
- text
- score from 0 to 1 indicating the presence of a sensitive topic:
  - real crime
  - online crime
  - drugs
  - gambling
  - pornography
  - prostitution
  - slavery
  - suicide
  - terrorism
  - weapons
  - body shaming
  - health shaming
  - politics
  - racism
  - religion
  - sexual minorities
  - sexism
  - social_injustice

The folder contains the following files:
- ``sensitive_topics.csv`` -- all data labelled for sensitive topics (33,303 instances)
- ``train.csv``, ``val.csv``, ``test.csv`` -- data separated into training, validation, and test subsets in proportion 80:10:10. 

We also provide scripts for training and running models on the dataset:
- ``Training.ipynb`` -- training of a model on the data
- ``Inference.ipynb`` -- running of the pre-trained model
- ``id2topic.json`` -- a convenience file for running predictions by the pre-trained model. It contains the mapping from ids assigned by the model to the labels.

The model trained on this data can be used via tranformes API as [Skoltech/russian-sensitive-topics](https://huggingface.co/Skoltech/russian-sensitive-topics). 
