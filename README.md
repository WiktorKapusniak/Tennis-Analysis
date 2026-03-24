<img width="1932" height="1087" alt="image" src="https://github.com/user-attachments/assets/fbcfbe04-ae85-460b-bbd4-ac03640b8810" /># Tennis Game Analysis with AI

An advanced computer vision project that leverages deep learning to automatically detect, track, and analyze tennis players and ball movements in video sequences. This system uses state-of-the-art YOLO models and keypoint detection to provide detailed insights into tennis gameplay.

# Screen of outpud video

## 🎯 Project Overview

This project implements a comprehensive tennis video analysis pipeline that:

- **Detects and tracks** both tennis players and the ball throughout a video
- **Identifies court geometry** using keypoint detection on the first frame
- **Analyzes ball trajectories** and detects hitting moments
- **Visualizes court perspective** with 3D mini-court representation
- **Generates annotated videos** showing all detections and analyses

Perfect for sports analytics, coaching analysis, and training feedback systems.

## ✨ Key Features

- **Player Detection & Tracking**: Real-time detection of tennis players using YOLOv8x with multi-frame tracking
- **Ball Tracking**: Specialized ball detection using custom YOLO model with trajectory interpolation
- **Court Line Detection**: ResNet50-based keypoint detection to identify all court boundaries and lines
- **Ball Shot Detection**: Intelligent analysis of ball trajectory to identify hitting moments
- **Mini Court Visualization**: 3D perspective view showing normalized player and ball positions on the court
- **Frame Annotation**: Comprehensive visualization with bounding boxes, keypoints, and tracking information
- **Stub Caching**: Efficient processing with cached detection results for faster iteration
- **Purpose**: Establishes court geometry for perspective transformation

## Training
Tennis ball detetcor with YOLO: training/tennis_ball_detector_training.ipynb
Tennis court keypoint with Pytorch: training/tennis_court_keypoints_training.ipynb

## Requirements
python3.8
ultralytics
pytroch
pandas
numpy
opencv
