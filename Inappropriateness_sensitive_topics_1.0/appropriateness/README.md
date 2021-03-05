**Appropriateness dataset**

The appropriateness dataset contains Russian sentences labelled for the appropriateness and the presence of sensitive topics. The files contain the following columns:
- text
- inappropriateness score (0 to 1)
- whether the topic was assigned manually or automatically (0/1)
- 18 sensitive topics (0/1 for each topic)
- no sensitive topic (0/1)
- toxicity score (0 to 1 assigned automatically)

The folder contains the following files:
- ``Appropriateness.csv`` -- all data labelled for the appropriateness (82,063 instances)
- ``train.csv``, ``val.csv``, ``test.csv`` -- data separated into training, validation, and test subsets in proportion 80:10:10. 

We also provide scripts for training and running models on the dataset:
- ``Inappropriateness_training.ipynb`` -- training of a model on the data
- ``Inappropriateness_classifier_inference.ipynb`` -- running of the pre-trained model

The model trained on this data can be downloaded [here](https://drive.google.com/file/d/1MRY9dIFllHH_aB0wgc2NLg2e3XCJUITm/view?usp=sharing). The ``Inappropriateness_classifier_inference.ipynb`` notebook contains the code for downloading the model.
