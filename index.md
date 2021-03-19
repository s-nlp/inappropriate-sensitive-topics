# Inappropriate Sensitive Topics

This repository contains two versions of two datasets of Russian texts. 
The first dataset is dedicated to sensitive topics which have a high chance of yielding a discussion which can harm the speaker’s reputation.
The second dataset is dedicted to inappropriate messages -- the messages on a sensitive topic which can frustrate the reader and/or harm the reputation of the speaker.
You can learn more information about the concept of sensitive topics and inappropriate messages in the pre-print of [our article](https://arxiv.org/abs/2103.05345) presented at the workshop for [Balto-Slavic NLP at EACL-2021 conference](http://bsnlp.cs.helsinki.fi/).

The datasets were manually labelled via Yandex.Toloka.
To the best of our knowledge, these are the first datasets with such labelling for Russian as well as any other languages.

[Version1](Version1)

This folder contains first version of the datasets.  The sensitive topicsdatasets consist of 25,679,  the inappropriate messages dataset consists of 82,063 samples.
This version of the datasets was presented at the workshop for Balto-Slavic NLP at EACL-2021 conference.

[Version2](Version2)

This folder containes final extended versions of sensitive topics and inappropriate messages datasets.
The final vesrion of sensitive topics dataset consists of 33303 samples, final version of inappropriate messages dataset consists of 163332 samples.

## Hugging Face model hub

We have released the models trained on both datasests in Hugging Face model hub.
The sensitive topics classifier can be found [here](https://huggingface.co/Skoltech/russian-sensitive-topics), inappropriateness classifier can be found [here](https://huggingface.co/Skoltech/inappropriate-messages-high-confidence)

## Citation

If you find this repository helpful, feel free to cite our publication:

```
@inproceedings{babakov-etal-2021-bsnlp,
    title = "Detecting Inappropriate Messages on Sensitive Topics that Could Harm a Company's Reputation",
    author = "Babakov, Nikolay and Logacheva, Varvara and Kozlova, Olga and Semenov, Nikita and Panchenko, Alexander",
    booktitle = "In the Proceedings of the 8th Workshop on Balto-Slavic Natural Language Processing (BSNLP)",
    month = April,
    year = "2021",
    address = "Kyiv, Ukraine"
}
```

## Contact

If you have any question about the system write an issue or drop an email to [Nikolay](mailto:N.Babakov@skoltech.ru)

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png
