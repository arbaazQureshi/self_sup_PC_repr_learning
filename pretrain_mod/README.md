## <h1 align="center">Pre-training</h1>

#### Table of contents
1. [Pre-training](#Pre-training)

## Pre-training
Run the following command to pre-train models with different backbones.
```bash
python train.py \
--num_views 12 \ # number of view used for each object
--num_point_contrast 512 \ # number of positive pair for contrastive loss
--num_points 1024 \ # number of points for each object
--dataset path_to_folder_dataset \
--log_dir path_to_result_model \
--path_model path_to_pre_trained_2d_image \
--model pointnet \ # pre-training backbone pointnet or dgcnn
--window_size=16
```


