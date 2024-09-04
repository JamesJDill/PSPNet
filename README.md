Semantic Segmentation using Deep Learning: PSPNet Architecture Implementation
---
## Environment Setup
  - install script  : conda/install.sh
  - requirement list: conda/requirements.txt

# Documentation
- Additional information can be found in `docs/implementation_details.pdf`.
- 
# Code/Directory Structure:

PSPNet
 * [conda](PSPNet/conda)
 * [dataset_lists](PSPNet/dataset_lists)
   * [camvid-11](PSPNet/dataset_lists/camvid-11)
     * [list](PSPNet/dataset_lists/camvid-11/list)
   * [kitti](PSPNet/dataset_lists/kitti)
 * [docs](PSPNet/docs)
 * [kitti](PSPNet/kitti)
   * [testing](PSPNet/kitti/testing)
     * [calib](PSPNet/kitti/testing/calib)
     * [gt_image_2](PSPNet/kitti/testing/gt_image_2)
     * [image_2](PSPNet/kitti/testing/image_2)
   * [training](PSPNet/kitti/training)
   * [calib](PSPNet/kitti/training/calib)
   * [gt_image_2](PSPNet/kitti/training/gt_image_2)
   * [image_2](PSPNet/kitti/training/image_2)
 * [src](PSPNet/src)
   * [dataset_lists](PSPNet/src/dataset_lists)
     * [camvid-11](PSPNet/src/dataset_lists/camvid-11)
       * [list](PSPNet/src/dataset_lists/camvid-11/list)
     * [kitti](PSPNet/src/dataset_lists/kitti)
   * [vision](PSPNet/src/vision)
   * [__pycache__](PSPNet/src/vision/__pycache__)
 * [tests](PSPNet/tests)
     * [__pycache__](PSPNet/tests/__pycache__)
     * [test_data](PSPNet/tests/test_data)
         * [CamvidSubsampled](PSPNet/tests/test_data/CamvidSubsampled)
             * [701_StillsRaw_full](PSPNet/tests/test_data/CamvidSubsampled/701_StillsRaw_full)
             * [semseg11](PSPNet/tests/test_data/CamvidSubsampled/semseg11)
