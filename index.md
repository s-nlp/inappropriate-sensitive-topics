# Inappropriate Sensitive Topics

This repository contains two versions of two datasets of Russian texts. 
The first dataset is dedicated to sensitive topics which have a high chance of yielding a discussion that can harm the speaker’s reputation.
The second dataset is dedicated to inappropriate messages -- the messages on a sensitive topic which can frustrate the reader and/or harm the reputation of the speaker.
You can learn more information about the concept of sensitive topics and inappropriate messages in the pre-print of [our article](https://arxiv.org/abs/2103.05345) presented at the workshop for [Balto-Slavic NLP at EACL-2021 conference](http://bsnlp.cs.helsinki.fi/).

The datasets were manually labeled via Yandex.Toloka.
To the best of our knowledge, these are the first datasets with such labeling for Russian as well as any other languages.

[Version1](https://github.com/skoltech-nlp/inappropriate-sensitive-topics/tree/main/Version1)

This folder contains the first version of the datasets.  The sensitive topic datasets consist of 25,679,  the inappropriate messages dataset consists of 82,063 samples.
This version of the datasets was presented at the workshop for Balto-Slavic NLP at EACL-2021 conference.

[Version2](https://github.com/skoltech-nlp/inappropriate-sensitive-topics/tree/main/Version2)

This folder contains final extended versions of sensitive topics and inappropriate messages datasets.
The final version of the sensitive topics dataset consists of 33,303 samples, final version of the inappropriate messages dataset consists of 163,332 samples.

The thorough statistics table of two versions of the Sensitive topics dataset (ST) and two versions of the Appropriateness utterances (AU) dataset is below. We specifically indicate the quantity of 100% confidence samples, because we released the model trained only on these samples because it demonstrated higher metrics. 

| Sensitive topic   | ST v1 | ST v2 | AU v1 | AU v2 | AU v2 100% confidence |
|-------------------|--------------|--------------|--------------------|--------------------|------------------------------------|
| <strong>total samples</strong>     |       <strong>25,679</strong>  |       <strong>33,033</strong>  |             <strong>82,063</strong>  |            <strong>163,332</strong>  |                            <strong>106,072</strong>  |
| body shaming      |          715 |        1,203 |              3,537 |              8,103 |                              5,621 |
| drugs             |        3,870 |        3,852 |              8,618 |              7,835 |                              5,197 |
| gambling          |        1,393 |        2,062 |              2,693 |              8,096 |                              5,278 |
| health shaming    |        1,744 |        1,731 |              7,270 |              7,945 |                              6,581 |
| offline crime     |        1,037 |        1,835 |              2,206 |              8,003 |                              4,893 |
| online crime      |        1,058 |        1,033 |              3,181 |              8,174 |                              4,238 |
| politics          |        1,593 |        2,155 |              7,650 |              7,105 |                              4,837 |
| pornography       |        1,289 |        2,002 |              2,824 |              7,889 |                              4,934 |
| prostitution      |          634 |        1,291 |                240 |              8,249 |                              4,924 |
| racism            |        1,156 |        1,572 |              3,760 |              6,816 |                              4,173 |
| religion          |        4,110 |        4,072 |              2,869 |              8,142 |                              4,478 |
| sexism            |        1,970 |        1,592 |                754 |              8,137 |                              4,883 |
| sexual minorities |        1,022 |        1,967 |              3,644 |              7,994 |                              3,985 |
| slavery           |          288 |        1,054 |                442 |              6,700 |                              3,793 |
| social injustice  |        1,230 |        1,875 |              5,294 |              7,494 |                              5,599 |
| suicide           |        1,420 |        1,407 |              1,931 |              6,425 |                              3,330 |
| terrorism         |          577 |        1,303 |                310 |              7,301 |                              3,394 |
| weapons           |        1,530 |        2,222 |                726 |              7,951 |                              4,327 |


## Hugging Face model hub

We have released the models trained on both datasets in Hugging Face model hub.
The sensitive topics classifier can be found [here](https://huggingface.co/Skoltech/russian-sensitive-topics), inappropriateness classifier can be found [here](https://huggingface.co/Skoltech/russian-inappropriate-messages)

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
