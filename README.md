# YOLO V7 Emotion Detection

## Overview

This project utilizes YOLO V7 for facial emotion detection from images and videos. The YOLO (You Only Look Once) algorithm is a real-time object detection system that can detect multiple objects in an image simultaneously.

## Emotion Classes

The model is trained to recognize the following emotion classes:

- Happy
- Sad
- Fear
- Anger
- Relax
- Worry
- Neutral
- Excited

Each emotion class consists of 500 images for training.

## Training Details

- **Training Duration**: 6 hours
- **Mean Average Precision (mAP)**: 0.75


## Project Structure

The project directory has the following structure:

- **best.pt**: Weights file containing the trained model for emotion detection.
- **confusion_matrix.png**: Confusion matrix image for evaluating model performance.
- **custom.yaml**: Configuration file for YOLO V7 customization.
- **F1_curve.png**: F1 score curve for model evaluation.
- **output1.txt**: Output file containing detected emotions.
- **PR_curve.png**: Precision-Recall curve image for model evaluation.
- **P_curve.png**: Precision curve image for model evaluation.
- **R_curve.png**: Recall curve image for model evaluation.
- **test.ipynb**: Jupyter notebook for testing and visualization.
- **detect.py**: Python script for detecting emotions using the trained model.
- **YOLOV7(Train).ipynb**: Jupyter notebook for training YOLO V7 on custom data.
- **runs**: Directory containing detection results.
  - **detect/exp**: Directory containing detected frames from the test set.

## How to Detect Emotions

To detect emotions, use the following command:

```bash
!python detect.py --weights /path/to/best.pt --img 480 --conf 0.40 --source "/path/to/source/images/folder"
```


- **weights**: Path to the trained model weights file (best.pt).
- **img**: Size of the input image for detection.
- **conf**: Confidence threshold for detection.
- **source**: Path to the source directory containing test images or videos.

## Results
The results of the emotion detection can be found in the runs/detect/exp directory. Detected frames are saved as image files.

## Evaluation
Model performance evaluation metrics, including confusion matrix and various curves, are available in the project directory.
