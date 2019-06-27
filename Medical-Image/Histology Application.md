### Histology Applicaition
---

**1. Skin Lesion Classification in Dermoscopy Images Using Synergic Deep Learning  MICCAI2018**

**Introduction**

In this paper, the author proposes an interesting structure with two convolutional networks to classify skin lesion into benign and malignancy.

**2. Collaborative Learning of Semi-Supervised Segmentation and Classification for Medical Images  CVPR2019**

**Summary**

This paper proposed a collaborative framework to unify segmentation and grading (classification) tasks. It uses a few pixel-level annotated images and lots of image-level annotated images to train this model. The two tasks boosts each other in the end-to-end training process. An attentive model is introduced in this framwork to generate better pesudo masks and classification results.

**Strengths**

- This paper combines segmentation and classification, which is interesting in medical domain due to lack of fine-grained annotations.
- The attentive module utilizes low level feature and high level feature at the same time to generate attention mask.
- This paper uses three datasets and leverages some preprocess method to unify their appearance.

**Weaknesses**

- This work uses pixel-level annotated images and image-level annotated images, which is easier than weakly supervised segmentation and semi-supervised segmentation. Only the interaction of the two tasks brings some new things.
- The collaborative framework share the same masks generator. Actually I don't think it's a real collaborative model.
- The attentive module is a little tricky. This paper doesn't explain why the attentive module should be designed in such a complex stucture. It seems the authors blindly try many structures and choose the one giving best results.
- The comapred methods don't use segmentation annotations and they also use different traning data.