**Tunnel Vision: A Deep Learning Technique for Accident Detection in Low-Quality CCTV Footage**
Tunnel Vision is a deep learning-based object detection system designed to detect and localize road accidents from low-quality tunnel CCTV footage. This project utilizes the Faster R-CNN architecture with a ResNet-50 backbone and Feature Pyramid Network (FPN) to accurately draw bounding boxes around accident zones in tunnel environments.

Problem Statement
Detecting accidents in tunnels is difficult due to low-light conditions, poor image quality, and limited camera perspectives. Traditional monitoring systems rely heavily on manual surveillance, which is prone to delays and human error.

🎯 Objective
To develop a robust object detection model capable of automatically identifying and localizing road accidents in CCTV images captured from tunnels, even under degraded image quality.

🔬 Methodology
Data Annotation: COCO-format annotations were created for tunnel CCTV images labeled as “accident” and “normal”.

Image Preprocessing: All images were resized to 640×640, and transformations were applied for normalization.

Model Selection: Used Faster R-CNN with ResNet-50 + FPN as the backbone.

Training: The model was trained using PyTorch with Adam optimizer and cross-entropy loss.

Evaluation & Inference: Predictions include bounding boxes, labels, and confidence scores. Only detections above a threshold (e.g., 0.5) are visualized.

🧠 Model Architecture
Backbone: ResNet-50

Feature Extractor: Feature Pyramid Network (FPN)

Detector: Faster R-CNN

Optimizer: Adam (Learning rate = 0.0001)

Loss Function: Classification (Cross Entropy) + Regression (Smooth L1)

🗂️ Dataset
Format: COCO JSON

Classes: Normal, Accident

Source: Custom annotated tunnel CCTV image dataset

Note: Dataset is not publicly shared due to privacy concerns. Replace with your own or contact for usage details.

Visualize Results:
Bounding boxes with class labels and confidence scores will be drawn on the images.

Results
Accurate accident localization using bounding boxes

Works effectively with low-resolution CCTV images

High precision in binary classification (accident vs normal)



📈 Results
Accurate accident localization using bounding boxes

Works effectively with low-resolution CCTV images

High precision in binary classification (accident vs normal)
