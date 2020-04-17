# Depth from Video in the Wild: Unsupervised Monocular Depth Learning from Unknown Cameras

Modified to apply for my own video


Input Example (20200312)

```script
nohup python -m depth_from_video_in_the_wild.train \
--data_dir /home/ubuntu/data/result_tokushima_dataprocessing3 \
--checkpoint_dir=/home/ubuntu/data/tokushima_checkpoint2 \
--img_height=192 \
--img_width=192 \
--train_steps=50000 &
```

