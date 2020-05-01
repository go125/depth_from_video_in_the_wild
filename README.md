# Depth from Video in the Wild: Unsupervised Monocular Depth Learning from Unknown Cameras

[Original](https://github.com/google-research/google-research/tree/master/depth_from_video_in_the_wild)

This code is modified to apply for my own video.

## Train example

Input Example (20200312_2)

```script
nohup python -m depth_from_video_in_the_wild.train \
--data_dir /home/ubuntu/data/result_tokushima_dataprocessing4 \
--checkpoint_dir=/home/ubuntu/data/cityscapes_kitti_learned_intrinsics \
--train_steps=1010000 &

```

## Evaluation (Under Construction)

### kitti_learned_intrinsics

```shell
python inference.py \
    --logtostderr \
    --file_extension png \
    --depth \
    --egomotion true \
    --input_list_file /home/ubuntu/data/raw_data_KITTI/test_files_eigen.txt \
    --output_dir /home/ubuntu/data/dfv_KITTI_depth_result_20200430_inv/ \
    --model_ckpt /home/ubuntu/data/kitti_learned_intrinsics/model-248900
```

### cityscapes_kitti_learned_intrinsics

```shell
python inference.py \
    --logtostderr \
    --file_extension png \
    --depth \
    --egomotion true \
    --input_list_file /home/ubuntu/data/raw_data_KITTI/test_files_eigen.txt \
    --output_dir /home/ubuntu/data/dfv_KITTI_depth_result_20200430_2/ \
    --model_ckpt /home/ubuntu/data/cityscapes_kitti_learned_intrinsics/model-1000977
```

You can get model from [here](https://github.com/google-research/google-research/tree/master/depth_from_video_in_the_wild).

After use this code, you can calculate Abs Rel Error using [this code](https://github.com/go125/SfmLearner_eval).

