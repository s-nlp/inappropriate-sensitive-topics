**Sensitive topics dataset**

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
- ``Sensitive_topics.csv`` -- all data labelled for sensitive topics (29,209 instances)
- ``Sensitive_topics_crowdsource_only.csv`` -- the subset of the data labelled by human workers 
- ``train.csv``, ``val.csv``, ``test.csv`` -- data separated into training, validation, and test subsets in proportion 80:10:10. 

We also provide scripts for training and running models on the dataset:
- ``Sensitive_topics_training.ipynb`` -- training of a model on the data
- ``Sensitive_inference.ipynb`` -- running of the pre-trained model
- ``target_vaiables_id2topic_dict.json`` -- a convenience file for running predictions by the pre-trained model. It contains the mapping from ids assigned by the model to the labels.

The pre-trained model trained on this data can be downloaded [here](https://drive.google.com/file/d/1u_g7CSJPYUHuRc6CaoLn1tKhJ6t8kQxF/view?usp=sharing). The ``Sensitive_inference.ipynb`` notebook contains the code for downloading the model.
