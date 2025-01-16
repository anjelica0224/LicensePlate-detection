
Object detection for license-plates :

#### GroundedDINO.ipynb
Detects and annotates license plates in images using GroundingDINO, a pre-trained object detection model. Images are processed with OpenCV, and detections are filtered based on confidence thresholds. The results, including bounding boxes are visualized and annotated using Supervision and plotted with Matplotlib. 

<img width="838" alt="image" src="https://github.com/user-attachments/assets/0e11db70-e2d3-4665-b494-4e29e3755701" />


#### autodistill.ipynb
license plate detection system using YOLOv8 - 
- Frame Extraction: Frames were extracted from traffic videos using MoviePy and FFmpeg.
- Dataset Labeling: Frames were labeled using Autodistill with GroundedSAM and GroundedDINO models.
- Dataset Organization: Labeled data was split into training, validation, and testing sets.
- Model Training: The YOLOv8 model was fine-tuned using the labeled dataset, saving weights, logs, and validation metrics.
- Inference: The trained model was evaluated on videos, generating annotated outputs with optimized detection thresholds.

To verify the effectiveness of the trained YOLOv8 model, an inference was run on a sample traffic video with a confidence value of 0.5, which means that only detections with a confidence score of 50% or higher were considered. This threshold balances precision and recall, ensuring that the detected license plates are reliable while trying to minimize the false positives. 

#### license.ipynb
a MobileNetV2-based model is used for license plate detection with TensorFlow 2 and TFLite. It involves setting up TensorFlow v2.8.0, fine-tuning the model,converting it to TFLite for efficient deployment, and running inference on test images with adjustable confidence thresholds for real-time detection.
