# Semantic Segmentation: PSPNet Architecture Implementation
---
## Environment Setup
  - install script: conda/install.sh
  - requirement list: conda/requirements.txt

## Documentation
- Background information can be found in `docs/implementation_details.pdf`.
- 3 Notebooks: notebook_colab.ipynb, notebook_kitti.ipynb, notebook_local.ipynb
- train/test data stored in kitti/
- source code in src/vision
- test code in src/tests

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
