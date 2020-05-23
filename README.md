# Depth from Video in the Wild: Unsupervised Monocular Depth Learning from Unknown Cameras

[Original](https://github.com/google-research/google-research/tree/master/depth_from_video_in_the_wild)

This code is modified to apply for my own video.

## Train example

[Data Preparation](https://github.com/go125/PrepareDataForDFV)

### Input Example

```script
nohup python -m depth_from_video_in_the_wild.train \
--data_dir ./depth_from_video_in_the_wild/data_example \
--checkpoint_dir=/home/ubuntu/data/example_experiment_checkpoint_20200501 \
--train_steps=100 &

```

```script
nohup python -m depth_from_video_in_the_wild.train \
--data_dir /home/ubuntu/data/kitti_result_all_20200501 \
--checkpoint_dir=/home/ubuntu/data/kitti_experiment_checkpoint_20200501 \
--train_steps=1000000 &

```

```script
nohup python -m depth_from_video_in_the_wild.train \
--data_dir /home/ubuntu/data/kitti_result_all_20200513 \
--checkpoint_dir=/home/ubuntu/data/kitti_experiment_checkpoint_20200523 \
--train_steps=1000000 &

```

## Evaluation


Please use [this code](https://github.com/go125/struct2depth_eval).

