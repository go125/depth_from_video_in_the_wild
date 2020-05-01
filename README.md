# Depth from Video in the Wild: Unsupervised Monocular Depth Learning from Unknown Cameras

[Original](https://github.com/google-research/google-research/tree/master/depth_from_video_in_the_wild)

This code is modified to apply for my own video.

## Train example

[Data Preparation](https://github.com/go125/PrepareDataForDFV)

### Input Example (20200312_2)

```script
nohup python -m depth_from_video_in_the_wild.train \
--data_dir /home/ubuntu/data/result_tokushima_dataprocessing4 \
--checkpoint_dir=/home/ubuntu/data/cityscapes_kitti_learned_intrinsics \
--train_steps=1010000 &

```

## Evaluation


Please use [this code](https://github.com/go125/struct2depth_eval).

