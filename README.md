# Anterior Chamber Angle Dataset

## Introduction

Anterior Chamber Angle Dataset (ACA dataset) is stored in Hierarchical Data Format (h5) format. They have undergone simple preprocessing, such as using YoLo detection to crop out the critical area, and uniformly changing the size of the image to $700\times2100$.

The dataset includes 3 different groups: (1) group 1 is training data including image-level labels and pixel-level labels; (2) group 2 is testing data including image-level labels and pixel-level labels; (3) group 3 is the index of images and the corresponding pixel-level labels, because only a part of the image has pixel-level labels.

Note that the preprocess_img in group 'test' is the pre-processed testing samples of our trained GCNet. If you want to test the performance of our model, you just need to convert the data to tensor format: [bs, c, h, w].

Below is the structure diagram of the h5 file, where label denote image-level label and mask denote pixel-level labels:

```
.
├── group1:training data
│   ├── img
│   ├── label
│   ├── mask
├── group2:testing data
│   ├── img
│   ├── label
│   ├── preprocess_img
├── group3:idex
│   ├── train_img
│   ├── test_img
│   ├── train_mask
│   ├── test_mask
└──
...
```

If you use ACA data for your research, please cite the following paper:

```
@InProceedings{aca_2022_cvpr,
author = {},
title = {},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {},
year = {2022}
}
```

## Download

Please provide us with your contact information to communicate future updates on the [dataset](https://drive.google.com/drive/folders/1S_tluE07ePE6nFFq3iUdOo5ar5eUKVJi?usp=sharing). The password for downloading the data will be shared with you once you submit **the Contact Information** and agree to **the Terms of Data Sharing and Usage** with your Signature to [jiaxp@gpnu.edu.cn](mailto:jiaxp@gpnu.edu.cn).

## Contact Information

First Name:

Last Name:

Affiliation:

Email address:

Terms of data sharing and usage:

I will not redistribute the dataset in any way and in any format. Any new access will be established through this form and/or authors' official method of releasing the dataset. I agree that the data and derivatives will be used only for non-commercial research and academic purposes.

## Contact

If any question, please contact [jiaxp@gpnu.edu.cn](mailto:jiaxp@gpnu.edu.cn).
