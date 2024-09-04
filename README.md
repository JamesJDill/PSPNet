Semantic Segmentation using Deep Learning: PSPNet Architecture Implementation
---
## Environment Setup
  - install script  : conda/install.sh
  - requirement list: conda/requirements.txt

## Project Structure
- Additional information can be found in `docs/implementation_details.pdf`.
.
├── README.md
├── conda
│   ├── environment.yml
│   ├── install.sh
│   └── requirements.txt
├── dataset_lists
│   └── camvid-11
│       ├── camvid-11_names.txt
│       └── list
│           ├── test.txt
│           ├── train.txt
│           └── val.txt
├── docs
│   └── implementation_details.pdf
├── download_dataset.sh
├── notebook_colab.ipynb
├── notebook_kitti_test.ipynb
├── notebook_local.ipynb
├── pyproject.toml
├── resnet50_v2.pth
├── setup.cfg
├── src
│   ├── dataset_lists
│   │   └── camvid-11
│   │       ├── camvid-11_names.txt
│   │       └── list
│   │           ├── test.txt
│   │           ├── train.txt
│   │           └── val.txt
│   └── vision
│       ├── __init__.py
│       ├── __pycache__
│       │   ├── __init__.cpython-310.pyc
│       │   ├── cv2_transforms.cpython-310.pyc
│       │   ├── iou.cpython-310.pyc
│       │   ├── part1_ppm.cpython-310.pyc
│       │   ├── part2_dataset.cpython-310.pyc
│       │   ├── part3_training_utils.cpython-310.pyc
│       │   ├── part4_segmentation_net.cpython-310.pyc
│       │   ├── part5_pspnet.cpython-310.pyc
│       │   ├── part6_transfer_learning.cpython-310.pyc
│       │   ├── resnet.cpython-310.pyc
│       │   └── utils.cpython-310.pyc
│       ├── accuracy_calculator.py
│       ├── avg_meter.py
│       ├── cv2_transforms.py
│       ├── dataset.py
│       ├── iou.py
│       ├── mask_utils.py
│       ├── ppm.py
│       ├── pspnet.py
│       ├── resnet.py
│       ├── segmentation_net.py
│       ├── test.py
│       ├── trainer.py
│       ├── training_utils.py
│       ├── transfer_learning.py
│       └── utils.py
├── kitti
│   ├── testing
│   └── training
└── tests
    ├── __init__.py
    ├── __pycache__
    │   ├── __init__.cpython-310.pyc
    │   ├── test_dataset.cpython-310-pytest-8.1.1.pyc
    │   ├── test_dataset.cpython-310.pyc
    │   ├── test_iou.cpython-310-pytest-8.1.1.pyc
    │   ├── test_kitti_dataset.cpython-310-pytest-8.1.1.pyc
    │   ├── test_kitti_dataset.cpython-310.pyc
    │   ├── test_ppm.cpython-310-pytest-8.1.1.pyc
    │   ├── test_ppm.cpython-310.pyc
    │   ├── test_pspnet.cpython-310-pytest-8.1.1.pyc
    │   ├── test_pspnet.cpython-310.pyc
    │   ├── test_segmentation_net.cpython-310-pytest-8.1.1.pyc
    │   ├── test_segmentation_net.cpython-310.pyc
    │   ├── test_training_utils.cpython-310-pytest-8.1.1.pyc
    │   └── test_training_utils.cpython-310.pyc
    ├── test_data
    │   ├── CamvidSubsampled
    │   │   ├── 701_StillsRaw_full
    │   │   │   ├── 0001TP_006690.png
    │   │   │   ├── 0001TP_006720.png
    │   │   │   └── 0001TP_006750.png
    │   │   └── semseg11
    │   │       ├── 0001TP_006690_L.png
    │   │       ├── 0001TP_006720_L.png
    │   │       └── 0001TP_006750_L.png
    │   └── dummy_camvid_train.txt
    ├── test_dataset.py
    ├── test_iou.py
    ├── test_kitti_dataset.py
    ├── test_ppm.py
    ├── test_pspnet.py
    ├── test_segmentation_net.py
    └── test_training_utils.py
