# 19th-century-fraktur-OCR
OCRopus/Calamari mixed models for recognizing (German) 19th century Fraktur scripts.

## Models
All models were trained on and should be applied to binary data since this showed the best results during evaluation (see [1]). We provide
* a Calamari voting ensemble consisting of five models (best results).
* a single Calamari model which should perform slightly better then each single model of the ensemble (if recognition time is a big issue).
* a OCRopus model.

## Data
At max 50 lines of each book in our training corpus are provided allowing to adapt the models to your own transcription guidelines.
Adjust the ground truth as desired and then train a new model using the provided models as a starting point (Calamari: --weights, OCRopus: --load).
For a description of the entire training data as well as a source for download please see [2].

## Related Publications

[1] Reul, Springmann, Wick, Puppe. (2018). 
State of the Art Optical Character Recognition of 19th Century Fraktur Scripts using Open Source Engines. Submitted to [DHd2019](https://dhd2019.org/). Preprint available at [ArXiv e-prints](https://arxiv.org/abs/1810.03436).

```
@article{reul2018fraktur,
  title = {State of the Art Optical Character Recognition of 19th Century Fraktur Scripts using Open Source Engines},
  author = {Reul, Christian and Springmann, Uwe and Wick, Christoph and Puppe, Frank},
  journal = {ArXiv e-prints},
  url = {https://arxiv.org/abs/1810.03436},
  year = {2018}
}

```

[2] Springmann, Reul, Dipper, Baiter. (2018). 
Ground Truth for training OCR engines on historical documents in German Fraktur and Early Modern Latin. Submitted to Submitted to JLCL Volume 33 (2018), Issue 1: Special Issue on Automatic Text and Layout Recognition. Preprint available at [ArXiv e-prints](https://arxiv.org/abs/1809.05501).

```
@article{springmann2018groundtruth,
  title = {Ground Truth for training OCR engines on historical documents in German Fraktur and Early Modern Latin},
  author = {Springmann, Uwe and Reul, Christian and Dipper, Stefanie and Baiter, Johannes},
  journal = {ArXiv e-prints},
  url = {https://arxiv.org/abs/1809.05501},
  year = {2018}
}
