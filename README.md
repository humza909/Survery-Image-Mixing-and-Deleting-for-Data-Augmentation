# Survery: Image Mixing and Deleting for Data Augmentation

This repo is for our paper: https://arxiv.org/abs/2106.07085 

[Humza Naveed](https://scholar.google.com.pk/citations?user=k5dpooQAAAAJ&hl=en), [Saeed Anwar](https://scholar.google.com.au/citations?user=vPJIHywAAAAJ&hl=en), [Munawar Hayat](https://scholar.google.com.au/citations?user=Mx8MbWYAAAAJ&hl=en), [Kashif Javed](https://scholar.google.com.pk/citations?user=yFxpLBwAAAAJ&hl=en), [Ajmal Mian](https://scholar.google.com/citations?user=X589yaIAAAAJ&hl=en)

## Contents
- [Abstract](#abstract)
- [Cut and Delete](#cut-and-delete)
- [Cut and Mix](#cut-and-mix)
- [Mix and Up](#mix-and-up)
- [Applications](#applications)
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

## Mix and Up

## Applications
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
