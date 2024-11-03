# Inappropriate Sensitive Topics

This repository contains two versions of two datasets of Russian texts. 
The first dataset is dedicated to sensitive topics which have a high chance of yielding a discussion which can harm the speaker’s reputation.
The second dataset is dedicted to inappropriate messages -- the messages on a sensitive topic which can frustrate the reader and/or harm the reputation of the speaker.
You can learn more information about the concept of sensitive topics and inappropriate messages in the pre-print of [our article](https://arxiv.org/abs/2103.05345) presented at the workshop for [Balto-Slavic NLP at EACL-2021 conference](http://bsnlp.cs.helsinki.fi/) and [Language Resources and Evaluation Journal](https://link.springer.com/article/10.1007/s10579-023-09682-z).

The datasets were manually labelled via Yandex.Toloka.
To the best of our knowledge, these are the first datasets with such labelling for Russian as well as any other languages.

[Version1](Version1)

This folder contains first version of the datasets.  The sensitive topicsdatasets consist of 25,679,  the inappropriate messages dataset consists of 82,063 samples.
This version of the datasets was presented at the workshop for Balto-Slavic NLP at EACL-2021 conference.

[Version2](Version2)

This folder containes final extended versions of sensitive topics and inappropriate messages datasets.
The final vesrion of sensitive topics dataset consists of 33303 samples, final version of inappropriate messages dataset consists of 163332 samples.

[Version3](Version3)

This is the final version of our dataset. Sensitive topics dataset still has 33,303 samples. Inappropriate messages dataset is shortened by confidence (we leave only the ones with 0.9 and above) and by agreement (we leave only the samples where either all or all but one annotators agree on the value of sample, it results in Krippendorf's alpha 0.65), so now it consists of 124,597 samples. This version of the datasets is presented to Language resources and Evaluation Journal, in the paper "Beyond plain toxic: building datasets for detection of flammable topics and inappropriate statements". 


## Hugging Face model hub

We have released the models trained on both datasests in Hugging Face model hub.
The sensitive topics classifier can be found [here](https://huggingface.co/Skoltech/russian-sensitive-topics), inappropriateness classifier can be found [here](https://huggingface.co/Skoltech/russian-inappropriate-messages)

## Citation

If you find this repository helpful, cite the following papers related to the dataset:
```
@article{babakov2024beyond,
  title={Beyond plain toxic: building datasets for detection of flammable topics and inappropriate statements},
  author={Babakov, Nikolay and Logacheva, Varvara and Panchenko, Alexander},
  journal={Language Resources and Evaluation},
  volume={58},
  number={2},
  pages={459--504},
  year={2024},
  publisher={Springer}
}
```

```
@inproceedings{babakov-etal-2021-detecting,
    title = "Detecting Inappropriate Messages on Sensitive Topics that Could Harm a Company{'}s Reputation",
    author = "Babakov, Nikolay  and
      Logacheva, Varvara  and
      Kozlova, Olga  and
      Semenov, Nikita  and
      Panchenko, Alexander",
    booktitle = "Proceedings of the 8th Workshop on Balto-Slavic Natural Language Processing",
    month = apr,
    year = "2021",
    address = "Kiyv, Ukraine",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2021.bsnlp-1.4",
    pages = "26--36",
    abstract = "Not all topics are equally {``}flammable{''} in terms of toxicity: a calm discussion of turtles or fishing less often fuels inappropriate toxic dialogues than a discussion of politics or sexual minorities. We define a set of sensitive topics that can yield inappropriate and toxic messages and describe the methodology of collecting and labelling a dataset for appropriateness. While toxicity in user-generated data is well-studied, we aim at defining a more fine-grained notion of inappropriateness. The core of inappropriateness is that it can harm the reputation of a speaker. This is different from toxicity in two respects: (i) inappropriateness is topic-related, and (ii) inappropriate message is not toxic but still unacceptable. We collect and release two datasets for Russian: a topic-labelled dataset and an appropriateness-labelled dataset. We also release pre-trained classification models trained on this data.",
}
```
## Contact

If you have any question about the system write an issue or drop an email to [Nikolay](mailto:N.Babakov@skoltech.ru)

## License
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png
