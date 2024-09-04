### Car Detection Using OpenCV and YOLOv3

This project demonstrates car detection in videos using the YOLOv3 (You Only Look Once, Version 3) model with OpenCV. YOLOv3 is a state-of-the-art real-time object detection algorithm that can identify multiple objects within a single image, making it suitable for tasks like car detection.

#### Key Components:
1. **YOLOv3 Weights and Config Files:** The pre-trained YOLOv3 weights (`yolov3.weights`) and configuration file (`yolov3.cfg`) are used for object detection. These files can be downloaded from the official YOLO website or GitHub repository.
2. **COCO Names File:** YOLOv3 is trained on the COCO dataset, so a `coco.names` file is required, which contains the list of all detectable objects, including "car."
3. **OpenCV for Video Processing:** OpenCV is utilized to process video frames in real time, allowing for frame-by-frame detection of cars.

#### How It Works:
- **Load Model:** The YOLOv3 model is loaded using OpenCV's DNN module. The weights, configuration file, and COCO names are provided to initialize the network.
- **Video Input:** The video file or stream is processed frame by frame.
- **Object Detection:** For each frame, YOLOv3 performs object detection. Bounding boxes are drawn around detected cars, and confidence scores are displayed.
- **Output:** The processed video can be saved or displayed, showing the detected cars in real time.

#### Prerequisites:
- Python 3.x
- OpenCV (`opencv-python`)
- Numpy (`numpy`)
- YOLOv3 weights and config files

#### Usage:
1. Download the required YOLOv3 files (`yolov3.weights`, `yolov3.cfg`, `coco.names`).
2. Install the necessary Python packages using `pip install opencv-python numpy`.
3. Run the script with the path to the video file as an argument.

```bash
python car_detection.py --video /path/to/video.mp4
```

#### References:
- [YOLOv3 Paper](https://arxiv.org/abs/1804.02767)
- [OpenCV Documentation](https://docs.opencv.org/4.x/d6/d0f/group__dnn.html)

