YOLO V7 Emotion Detection
Overview
This project utilizes YOLO V7 for facial emotion detection from images and videos. The YOLO (You Only Look Once) algorithm is a real-time object detection system that can detect multiple objects in an image simultaneously.

Project Structure
The project directory has the following structure:

best.pt: Weights file containing the trained model for emotion detection.
confusion_matrix.png: Confusion matrix image for evaluating model performance.
custom.yaml: Configuration file for YOLO V7 customization.
F1_curve.png: F1 score curve for model evaluation.
output1.txt: Output file containing detected emotions.
PR_curve.png: Precision-Recall curve image for model evaluation.
P_curve.png: Precision curve image for model evaluation.
R_curve.png: Recall curve image for model evaluation.
test.ipynb: Jupyter notebook for testing and visualization.
detect.py: Python script for detecting emotions using the trained model.
YOLOV7(Train).ipynb: Jupyter notebook for training YOLO V7 on custom data.
runs: Directory containing detection results.
detect/exp: Directory containing detected frames from the test set.
How to Detect Emotions
To detect emotions, use the following command:
