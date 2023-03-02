
# Social Distancing Detector

This is a Python project that detects social distancing violations in videos using computer vision techniques. The project takes a video as input and outputs a new video with bounding boxes around people, colored green if they are socially distant and red if they are too close together. In addition, the project plays an alert sound when a violation occurs.

## Requirements

- Python 3.6 or higher
- OpenCV
- Numpy
- Playsound

## Installation

Clone the repository to your local machine.
Install the required libraries using pip:

```bash
pip install opencv-python numpy playsound
```

## Usage

Place your input video file in the input directory.
Run the social_distance_detector.py script:

To run requires "coco.names", "yolov3.cfg", and "yolov3.weights" inside a folder (yolo-coco).  
you can download YOLOfrom here: https://pjreddie.com/darknet/yolo/

```bash
python social_distance_detector.py --input input/my_video.mp4 --output output/my_video_output.mp4
```

The output video with the detected social distancing violations will be saved to the output directory. In addition, an alert sound will play whenever a violation is detected.

## Customization

The project can be customized to meet your specific requirements. For example, you can adjust the minimum distance between people to be considered socially distant or change the alert sound. These options can be passed as command-line arguments to the social_distance_detector.py script.

Here's an example of how to change the minimum distance:

```bash
python social_distance_detector.py --input input/my_video.mp4 --output output/my_video_output.mp4 --min-distance 100
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

Contributions are welcome! Please feel free to open a pull request or issue if you have any suggestions or find any bugs.





