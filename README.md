# Survery: Image Mixing and Deleting for Data Augmentation

This repo is for our paper: https://arxiv.org/abs/2106.07085 

[Humza Naveed](https://scholar.google.com.pk/citations?user=k5dpooQAAAAJ&hl=en), [Saeed Anwar](https://scholar.google.com.au/citations?user=vPJIHywAAAAJ&hl=en), [Munawar Hayat](https://scholar.google.com.au/citations?user=Mx8MbWYAAAAJ&hl=en), [Kashif Javed](https://scholar.google.com.pk/citations?user=yFxpLBwAAAAJ&hl=en), [Ajmal Mian](https://scholar.google.com/citations?user=X589yaIAAAAJ&hl=en)

We intend to regularly update this repo with new papers. If you see any paper missing here, please create an issue or PR. 

## Contents
- [Abstract](#abstract)
- [Cut and Delete](#cut-and-delete)
- [Cut and Mix](#cut-and-mix)
- [Mix and Up](#mix-and-up)
- [Applications](#applications)
  - [Fine Grained Image Recognition](#fine-grained-image-recognition)
  - [Object Detection](#object-detection)
  - [Transformers](#transformers)
  - [Self-Supervised Learning](#self-supervised-learning)
  - [Semi-Supervised Learning](#semi-supervised-learning)
  - [Unsupervised Learning](#unsupervised-learning)
  - [Adversarial Training](#adversarial-training)
  - [Privacy Preserving](#privacy-preserving)
  - [Point Clouds](#point-clouds)
  - [Text Classification](#text-classification)
  - [Audio Classification](#audio-classification)
## Abstract
Neural networks are prone to overfitting and memorizing data patterns. To avoid over-fitting, and enhance
their generalization and performance, various methods have been suggested in the literature, including
dropout, regularization, label smoothing, etc. One such method is augmentation which introduces different
types of corruption in the data to prevent the model from overfitting and memorizing patterns present in
the data. A sub-area of data augmentation is image mixing and deleting. This specific type of augmentation
either deletes image regions or mixes two images to hide or make particular characteristics of images confusing
for the network, forcing it to emphasize the overall structure of the object in an image. Models trained with
this approach have proven to perform and generalize well compared to those trained without image mixing or
deleting. An added benefit that comes with this method of training is robustness against image corruption.
Due to its low computational cost and recent success, researchers have proposed many image mixing and
deleting techniques. We furnish an in-depth survey of image mixing and deleting techniques and provide
categorization via their most distinguishing features. We initiate our discussion with some fundamental
relevant concepts. Next, we present essentials, such as each category’s strengths and limitations, describing
their working mechanism, basic formulations, and applications. We also discuss the general challenges and
recommend possible future research directions for image mixing and deleting data augmentation techniques.

## Cut and Delete
* Improved regularization of convolutional neural networks with cutout, arXiv, 2017. [[Paper](https://arxiv.org/abs/1708.04552)] [[Code](https://github.com/uoguelph-mlrg/Cutout)]
* Hide-and-seek: Forcing a network to be meticulous for weakly-supervised object and action localization, ICCV, 2017. [[Paper](https://arxiv.org/abs/1704.04232)] [[Code](https://github.com/kkanshul/Hide-and-Seek)]
* Random erasing data augmentation, AAAI, 2020. [[Paper](https://arxiv.org/abs/1708.04896)] [[Code](https://github.com/zhunzhong07/Random-Erasing)]
* Gridmask data augmentation, arXiv, 2020. [[Paper](https://arxiv.org/abs/2001.04086)] [[Code](https://github.com/dvlab-research/GridMask)]

## Cut and Mix
* Ricap: Random image cropping and patching data augmentation for deep cnns, ACML, 2018. [[Paper](https://arxiv.org/abs/1811.09030)] [[Code](https://github.com/4uiiurz1/pytorch-ricap)]
* Improved mixed example data augmentation, WACV, 2019. [[Paper](https://arxiv.org/abs/1805.11272)] [[Code](https://github.com/ceciliaresearch/MixedExample)]
* Cutmix: Regularization strategy to train strong classifiers with localizable features, ICCV, 2019. [[Paper](https://arxiv.org/abs/1905.04899)] [[Code](https://github.com/clovaai/CutMix-PyTorch)]
* Resizemix: Mixing data with preserved object information and true labels, arXiv, 2020. [[Paper](https://arxiv.org/abs/2012.11101)]
* Attentive cutmix: An enhanced data augmentation approach for deep learning based image classification, ICASSP, 2020. [[Paper](https://arxiv.org/abs/2003.13048)]
* Saliencymix: A saliency guided data augmentation strategy for better regularization, ICLR, 2021. [[Paper](https://arxiv.org/abs/2006.01791)] [[Code](https://github.com/afm-shahab-uddin/SaliencyMix)]
* Keepaugment: A simple information-preserving data augmentation approach, CVPR, 2021. [[Paper]()] [[Code]()]
* Milking cowmask for semi-supervised image classification, VISIGRAPP, 2022. [[Paper](https://arxiv.org/abs/2003.12022)] [[Code](https://github.com/google-research/google-research/tree/master/milking_cowmask)]
* Recursivemix: Mixed learning with history, NeurIPS, 2022. [[Paper](https://arxiv.org/abs/2203.06844)] [[Code](https://github.com/implus/RecursiveMix-pytorch)]
* Lumix: Improving mixup by better modelling label uncertainty, arXiv, 2022. [[Paper](https://arxiv.org/abs/2211.15846)]
* Saliency grafting: Innocuous attribution-guided mixup with calibrated label mixing, AAAI, 2022. [[Paper](https://arxiv.org/abs/2112.08796)]
## Mix and Up
* Data augmentation by pairing samples for images classification, arXiv, 2018. [[Paper]()] [[Code]()]
* mixup: Beyond empirical risk minimizatio, ICLR, 2018. [[Paper]()] [[Code]()]
* Manifold mixup: Better representations by interpolating hidden states, ICML, 2019. [[Paper]()] [[Code]()]
* Remix: Rebalanced mixup, ECCV, 2020. [[Paper]()] [[Code]()]
* Augmix: A simple data processing method to improve robustness and uncertainty, ICLR, 2020. [[Paper]()] [[Code]()]
* Smoothmix: A simple yet effective data augmentation to train robust classifiers, CVPRW, 2020. [[Paper]()] [[Code]()]  
* Puzzle mix: Exploiting saliency and local statistics for optimal mixup, ICML, 2020. [[Paper]()] [[Code]()]
* Co-mixup: Saliency guided joint mixup with supermodular diversity, ICLR, 2021. [[Paper]()] [[Code]()]
* Supermix: Supervising the mixing data augmentation, CVPR, 2021. [[Paper]()] [[Code]()]
* Stylemix: Separating content and style for enhanced data augmentation, CVPR, 2021. [[Paper]()] [[Code]()]
* Automix: Unveiling the power of mixup for stronger classifier, ECCV, 2022. [[Paper]()] [[Code]()]
* Noisy feature mixup, ICLR, 2022. [[Paper]()] [[Code]()]
* Pixmix: Dreamlike pictures comprehensively improve safety measures, CVPR, 2022. [[Paper]()] [[Code]()]
* Alignmixup: Improving representations by interpolating aligned features, CVPR, 2022. [[Paper]()] [[Code]()]
## Applications
### Fine Grained Image Recognition
### Object Detection
### Transformers
### Self-Supervised Learning
### Semi-Supervised Learning
### Unsupervised Learning
### Adversarial Training
### Privacy Preserving
### Point Clouds
### Text Classification
### Audio Classification
# Citation
If you find this paper useful in your research, please cite the paper:

```
@article{naveed2021survey,
  title={Survey: Image mixing and deleting for data augmentation},
  author={Naveed, Humza and Anwar, Saeed and Hayat, Munawar and Javed, Kashif and Mian, Ajmal}, 
  journal={arXiv preprint arXiv:2106.07085},
  url = {https://arxiv.org/abs/2106.07085},
  year={2021}
}
```
