Deep learning for MS lesion segmentation
========================================================
author: Karma Tarap & Alexander Noll
date: 14-12-17
autosize: true


Multiple sclerosis & MRI
========================================================

Multiple sclerosis is a brain disease characterized by recurring or progressive **lesions** on white matter

Can be seen on **MRI scans**

Automatic segmentation would have important applications in diagnosing and monitoring the disease

Multiple sclerosis & MRI
========================================================

![](./lesion_unlabelled.png)
![](./lesion_3d_unlabelled.png)


Multiple sclerosis & MRI
========================================================

![](./lesion.png)
![](lesion_3d_labelled.png)

Difficulty of MRI segmentation
========================================================

+ MRIs are expensive
+ MRIs are big ($512 \times 512 \times 512$ voxels)
+ Physicians are expensive
+ Class imbalance (1.5% of brain mass for patients experiencing a lesion)

$\Longrightarrow$ Export annotation for supervised learning is not feasible, thus we are left with very few annotated MRI scans


Deep learning for lesion segmentation
========================================================

Similar to image segmentation: work with **3D convolutional neural networks** and classify each voxel individually: direct segmentation very hard because of small training set (20 MRIs)

Enhance data with **Generative adverserial networks** and use **semi-supervised learning**

Semi-supervised learning
========================================================

Use **combination** of **labelled** and **unlabelled** data

Build classifier to distinguish labelled from unlabelled data and distinguish labels between each other:

+ Binary classifier lesion vs non-lesion becomes
+ Trinary classifier lesion vs non-lesion vs unlabelled

Results & Outlook
========================================================

- Trained GAN to generate additional patches of lesions
- Set up pipeline for model tuning
- Experiencing difficulties training the classification model
  - Weak signal or bug in pipeline?

- Future work :
  - incorporate GAN directly into classifier
  - add more data sources
