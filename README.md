[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com) 
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/humza909/Survery-Image-Mixing-and-Deleting-for-Data-Augmentation)

# Survey: Image Mixing and Deleting for Data Augmentation

This repo supplements our paper: https://arxiv.org/abs/2106.07085 

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
* Data augmentation by pairing samples for images classification, arXiv, 2018. [[Paper](https://arxiv.org/abs/1801.02929)]
* mixup: Beyond empirical risk minimization, ICLR, 2018. [[Paper](https://arxiv.org/abs/1710.09412)] [[Code](https://github.com/facebookresearch/mixup-cifar10)]
* Manifold mixup: Better representations by interpolating hidden states, ICML, 2019. [[Paper](https://arxiv.org/abs/1806.05236)] [[Code](https://github.com/vikasverma1077/manifold_mixup)]
* Remix: Rebalanced mixup, ECCV, 2020. [[Paper](https://arxiv.org/abs/2007.03943)]
* Augmix: A simple data processing method to improve robustness and uncertainty, ICLR, 2020. [[Paper](https://arxiv.org/abs/1912.02781)] [[Code](https://github.com/google-research/augmix)]
* Smoothmix: A simple yet effective data augmentation to train robust classifiers, CVPRW, 2020. [[Paper](https://openaccess.thecvf.com/content_CVPRW_2020/papers/w45/Lee_SmoothMix_A_Simple_Yet_Effective_Data_Augmentation_to_Train_Robust_CVPRW_2020_paper.pdf)]  
* Puzzle mix: Exploiting saliency and local statistics for optimal mixup, ICML, 2020. [[Paper](https://arxiv.org/abs/2009.06962)] [[Code](https://github.com/snu-mllab/PuzzleMix)]
* Co-mixup: Saliency guided joint mixup with supermodular diversity, ICLR, 2021. [[Paper](https://arxiv.org/abs/2102.03065)] [[Code](https://github.com/snu-mllab/Co-Mixup)]
* Supermix: Supervising the mixing data augmentation, CVPR, 2021. [[Paper](https://arxiv.org/abs/2003.05034)] [[Code](https://github.com/alldbi/SuperMix)]
* Stylemix: Separating content and style for enhanced data augmentation, CVPR, 2021. [[Paper](https://openaccess.thecvf.com/content/CVPR2021/html/Hong_StyleMix_Separating_Content_and_Style_for_Enhanced_Data_Augmentation_CVPR_2021_paper.html)] [[Code](https://github.com/alsdml/StyleMix)]
* Automix: Unveiling the power of mixup for stronger classifier, ECCV, 2022. [[Paper](https://arxiv.org/abs/2103.13027)] [[Code](https://github.com/Westlake-AI/AutoMix)]
* Noisy feature mixup, ICLR, 2022. [[Paper](https://arxiv.org/abs/2110.02180)] [[Code](https://github.com/erichson/NFM)]
* Pixmix: Dreamlike pictures comprehensively improve safety measures, CVPR, 2022. [[Paper](https://arxiv.org/abs/2112.05135)] [[Code](https://github.com/andyzoujm/pixmix)]
* Alignmixup: Improving representations by interpolating aligned features, CVPR, 2022. [[Paper](https://arxiv.org/abs/2103.15375)] [[Code](https://github.com/shashankvkt/AlignMixup_CVPR22)]
## Applications
### Fine Grained Image Recognition
* Attribute mix: semantic data augmentation for fine grained recognition, VCIP, 2020. [[Paper](https://arxiv.org/abs/2004.02684)]
* Intra-class part swapping for fine-grained image classification, WACV, 2021. [[Paper](https://openaccess.thecvf.com/content/WACV2021/papers/Zhang_Intra-Class_Part_Swapping_for_Fine-Grained_Image_Classification_WACV_2021_paper.pdf)]
* Snapmix: Semantically proportional mixing for augmenting fine-grained data, AAAI, 2021. [[Paper](https://arxiv.org/abs/2012.04846)] [[Code](https://github.com/Shaoli-Huang/SnapMix)]
### Object Detection
* A-fast-rcnn: Hard positive generation via adversary for object detection, CVPR, 2017. [[Paper](https://arxiv.org/abs/1704.03414)] [[Code](https://github.com/xiaolonw/adversarial-frcnn)]
* Cut, paste and learn: Surprisingly easy synthesis for instance detection, ICCV, 2017. [[Paper](https://arxiv.org/abs/1708.01642)] [[Code](https://github.com/debidatta/syndata-generation)]
* Modeling visual context is key to augmenting object detection datasets, ECCV, 2018. [[Paper](https://arxiv.org/abs/1807.07428)] [[Code](https://github.com/dvornikita/context_aug)]
* Instant-Teaching: An End-to-End Semi-Supervised Object Detection Framework, CVPR, 2021. [[Paper](https://openaccess.thecvf.com/content/CVPR2021/html/Zhou_Instant-Teaching_An_End-to-End_Semi-Supervised_Object_Detection_Framework_CVPR_2021_paper.html
)] 
### Transformers
* Transmix: Attend to mix for vision transformers, CVPR, 2022. [[Paper](https://arxiv.org/abs/2111.09833)] [[Code](https://github.com/Beckschen/TransMix)]
* Tokenmix: Rethinking image mixing for data augmentation in vision transformers, ECCV, 2022. [[Paper](https://arxiv.org/abs/2207.08409)] [[Code](https://github.com/Sense-X/TokenMix)]
* Tokenmixup: Efficient attention-guided token-level data augmentation for transformers, NeurIPS, 2022. [[Paper](https://arxiv.org/abs/2210.07562)] [[Code](https://github.com/mlvlab/TokenMixup)]
### Self-Supervised Learning
* Improving contrastive learning by visualizing feature transformation, ICCV, 2021. [[Paper](https://arxiv.org/abs/2108.02982)] [[Code](https://github.com/DTennant/CL-Visualizing-Feature-Transformation)]
* i-mix: A domain-agnostic strategy for contrastive representation learning, ICLR, 2021. [[Paper](https://arxiv.org/abs/2010.08887)] [[Code](https://github.com/kibok90/imix)]
* A simple data mixing prior for improving self-supervised learning, CVPR, 2022. [[Paper](https://arxiv.org/abs/2206.07692)] [[Code](https://github.com/OliverRensu/SDMP)]
### Semi-Supervised Learning
* Mixmatch: A holistic approach to semi-supervised learning, NeurIPS, 2019. [[Paper](https://arxiv.org/abs/1905.02249)] [[Code](https://github.com/google-research/mixmatch)] 
* Remixmatch: Semi-supervised learning with distribution matching andaugmentation anchoring, ICLR, 2020. [[Paper](https://arxiv.org/abs/1911.09785)] [[Code](https://github.com/google-research/remixmatch)]
* Dividemix: Learning with noisy labels as semi-supervised learning, ICLR, 2020. [[Paper](https://arxiv.org/abs/2002.07394)] [[Code](https://github.com/LiJunnan1992/DivideMix)]
* Focalmix: Semi-supervised learning for 3d medical image detection, CVPR, 2020. [[Paper](https://arxiv.org/abs/2003.09108)]
* Fix-match: Simplifying semi-supervised learning with consistency and confidence, NeurIPS, 2020. [[Paper](https://arxiv.org/abs/2001.07685)] [[Code](https://github.com/google-research/fixmatch)]
### Unsupervised Learning
* Virtual mixup training for unsupervised domain adaptation, arXiv, 2019. [[Paper](https://arxiv.org/abs/1905.04215)] [[Code](https://github.com/xudonmao/VMT)]
* Improve unsupervised domain adaptation with mixup training, arXiv, 2020. [[Paper](https://arxiv.org/abs/2001.00677)]
* Fixbi:Bridging domain spaces for unsupervised domain adaptation, CVPR, 2021. [[Paper](https://arxiv.org/abs/2011.09230)] [[Code](https://github.com/NaJaeMin92/FixBi)]
* Center-wise local image mixture for contrastive representation learning, BMVC, 2021. [[Paper](https://arxiv.org/abs/2011.02697)]
* Un-mix: Rethinking image mixtures for unsupervised visual representation learning, AAAI, 2022. [[Paper](https://arxiv.org/abs/2003.05438)] [[Code](https://github.com/szq0214/Un-Mix)]
### Adversarial Training
* Inter-polated adversarial training: Achieving robust neural networks without sacrificing too much accuracy, AISec@CCS, 2019. [[Paper](https://arxiv.org/abs/1906.06784)] [[Code](https://github.com/shivamsaboo17/ManifoldMixup)]
* Adversarial vertex mixup: Toward better adversarially robust generalization, CVPR, 2020. [[Paper](https://arxiv.org/abs/2003.02484)] [[Code](https://github.com/hirokiadachi/Adversarial-vertex-mixup-pytorch)]
* Strong data augmentation sanitizes poisoning and backdoor attacks without an accuracy tradeoff, ICASSP, 2021. [[Paper](https://arxiv.org/abs/2011.09527)]
* Dp-instahide: Provably defusing poisoning and backdoor attacks with differentially private data augmentations, arXiv, 2021. [[Paper](https://arxiv.org/abs/2103.02079)]
### Privacy Preserving
* Instahide: Instance-hiding schemes for private distributed learning, ICML, 2020. [[Paper](https://arxiv.org/abs/2010.02772)] [[Code](https://github.com/Hazelsuko07/InstaHide)]
* Datamix: Efficient privacy-preserving edge-cloud inference, ECCV, 2020. [[Paper](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560562.pdf)]
* Xor mixup: Privacy-preserving data augmentation for one-shot federated learning, arXiv, 2020. [[Paper](https://arxiv.org/abs/2006.05148)] [[Code](https://github.com/ihooni/XOR-Mixup)]
### Point Clouds
* Pointmixup: Augmentation for point clouds, ECCV, 2020. [[Paper](https://arxiv.org/abs/2008.06374)] [[Code](https://github.com/yunlu-chen/PointMixup)]
* Regularization strategy for point cloud via rigidly mixed sample, CVPR, 2021. [[Paper](https://arxiv.org/abs/2102.01929)] [[Code](https://github.com/dogyoonlee/RSMix)]
* Pointcutmix: Regularization strategy for point cloud classification, Neurocomputing, 2022. [[Paper](https://arxiv.org/abs/2101.01461)] [[Code](https://github.com/cuge1995/PointCutMix)]
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
