# Object Detection with YOLOv2
**Final project** by Group 2 (Localization) in **Innovation & Practice Course** (2018, Spring).

## Inspiration
This repo [Car-detection-PA](https://github.com/n3rdd/Car-detection-PA) contains a tutorial for **YOLOv2**, which is a programming assignment in [Convolutional Neural Networks](https://www.coursera.org/learn/convolutional-neural-networks/) by Andrew Ng. 

## Requirements
- [Keras](https://github.com/fchollet/keras)
- [Tensorflow](https://www.tensorflow.org/) (For Keras backend.)
- [OpenCV](https://pypi.org/project/opencv-python/)
- [Numpy](http://www.numpy.org/)
- [h5py](http://www.h5py.org/) (For Keras model serialization.)
- [Python 3](https://www.python.org/)

## Installation 
Use `pip` to install the required packages in your command line. Visit the official sites above for more details.
```bash
pip install numpy h5py
pip install tensorflow
pip install keras
pip install opencv-python
```

## Quick Start
- [Download](https://pan.baidu.com/s/1sos5oov7V3O0uwOjoUvbuQ)(Password:8kim) `yolo.h5` in `model_data`
- Put your test image/video in `images/` or `videos/`
- Set your image/video file name and shape in `yolo_v2.py`
```python
if __name__ == '__main__':
    '''
    code
    '''
    # Set the original image/video shape
    image_shape = (960., 544.) # (height, width)
    
    # Detect a video
    video_file = "traffic.mp4"
    predict_video(sess, video_file)

    # Uncomment the code below to detect an image
    # out_scores, out_boxes, out_classes = predict_image(sess, "person.jpg")
```
- Run the model in your command line.
```bash
python yolo_v2.py
```
- The prediction info will be printed into `output.txt`.
- The notebook version will be uploaded very soon.


## More Details
// todo

## TODOs
- Unify the interface in the video detection part.
- Train the model.
- Try YOLOv3.
- ...


## Reference
- Joseph Redmon, Santosh Divvala, Ross Girshick, Ali Farhadi - [You Only Look Once: Unified, Real-Time Object Detection](https://arxiv.org/abs/1506.02640) (2015)
- Joseph Redmon, Ali Farhadi - [YOLO9000: Better, Faster, Stronger](https://arxiv.org/abs/1612.08242) (2016)
- Allan Zelener - [YAD2K: Yet Another Darknet 2 Keras](https://github.com/allanzelener/YAD2K)
- The official YOLO website (https://pjreddie.com/darknet/yolo/) 

