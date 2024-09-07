# Semantic Segmentation: [PSPNet](https://paperswithcode.com/method/pspnet)
---
Introduced by Zhao et al. in [Pyramid Scene Parsing Network](https://paperswithcode.com/paper/pyramid-scene-parsing-network).

**PSPNet**, or **Pyramid Scene Parsing Network**, is a semantic segmentation model that utilizes a pyramid parsing module that exploits global context information by different-region based context aggregation. The local and global clues together make the final prediction more reliable. We also propose an optimization.

Given an input image, PSPNet use a pretrained CNN with the dilated network strategy to extract the feature map. The final feature map size is **1/8** of the input image. On top of the map, we use the [Pyramid Pooling Module](https://paperswithcode.com/method/pyramid-pooling-module) to gather context information. Using our 4-level pyramid, the pooling kernels cover the whole, half of, and small portions of the image. They are fused as the global prior. Then we concatenate the prior with the original feature map in the final part of. It is followed by a convolution layer to generate the final prediction map.

![pspnet_image](https://github.com/user-attachments/assets/d3453661-b836-44e5-97f8-d9f951255945)

## Directory Information
- More Background information can be found in `docs/implementation_details.pdf`.
- 3 Notebooks: notebook_colab.ipynb, notebook_kitti.ipynb, notebook_local.ipynb
- train/test data stored in kitti/
- source code in src/vision
- test code in src/tests
  
## Environment Setup
  - install script: conda/install.sh
  - requirement list: conda/requirements.txt

## Directory Structure:
```
PSPNet
├── conda
├── dataset_lists
│   ├── camvid-11
│   │   └── list
│   └── kitti
├── docs
├── kitti
│   ├── testing
│   │   ├── calib
│   │   ├── gt_image_2
│   │   └── image_2
│   └── training
│       ├── calib
│       ├── gt_image_2
│       └── image_2
├── src
│   ├── dataset_lists
│   │   ├── camvid-11
│   │   │   └── list
│   │   └── kitti
│   └── vision
│       └── __pycache__
└── tests
    ├── __pycache__
    └── test_data
        └── CamvidSubsampled
            ├── 701_StillsRaw_full
            └── semseg11
```
