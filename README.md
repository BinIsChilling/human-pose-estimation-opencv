# human-pose-estimation-opencv
Perform Human Pose Estimation in OpenCV Using OpenPose MobileNet

![OpenCV Using OpenPose MobileNet](output.JPG)


# How to use

- Test with webcam

```
python openpose.py
```

- Test with image
```
python openpose.py --input image.jpg
```

- Use `--thr` to increase confidence threshold

```
python openpose.py --input image.jpg --thr 0.5
```

# Notes:
- Ensure that the TensorFlow model file (graph_opt.pb) is correctly specified in your working directory.
- The program is designed to capture video frames either from a specified file or directly from a camera. Ensure the input source is correctly set when running the script.
- Adjust the threshold (--thr) and width/height parameters when running the script to optimize performance for different environments or video resolutions.
- Run this script from the command line, passing in the appropriate arguments [python openpose.py --input video.mp4 --thr 0.3 --width 640 --height 480
]