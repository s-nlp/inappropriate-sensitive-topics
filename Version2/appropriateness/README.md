## Appropriateness dataset

The appropriateness dataset contains Russian sentences labelled for the appropriateness and the presence of sensitive topics. The files contain the following columns:
- text
- inappropriateness score (0 to 1)
- human_labeled - whether the topic was assigned manually or automatically (0/1)
- 18 sensitive topics (0/1 for each topic)
- none - no sensitive topic (0/1)
- toxicity score (0 to 1 assigned automatically)

The folder contains the following files:
- ``Appropriateness.csv`` -- all data labelled for the appropriateness (163,332 instances)
- ``train.csv``, ``val.csv``, ``test.csv`` -- data separated into training, validation, and test subsets in proportion 80:10:10. 
- ``Stratify.ipynb`` -- shows the process of the data stratification
- 
We also provide scripts for training and running models on the dataset:
- ``Training.ipynb`` -- training of a model on the data
- ``Inference.ipynb`` -- running of the pre-trained model

We also manually created list of appropriate and inappropriate samples ``manual_labelled.csv`` and compared our models performance with another existing classic toxic model with this data in ``compare_manual_data.ipynb``

The model trained on 100% confidence samples from this data can be used via tranformes API as [Skoltech/russian-inappropriate-messages](https://huggingface.co/Skoltech/russian-inappropriate-messages). 
