# Real World Marine Markers Custom Dataset YOLOv5 Training

## Welcome
Welcome to the *real_world_marine_markers_custom_dataset_yolov5_training* repository!This project focuses on training YOLOv5 models using a custom dataset of real-life images of marine markers for the [Roboboat](https://robonation.org/programs/roboboat/) compettion. Our objective is to enhance object detection in marine environments, contributing to safer marine navigation and advanced research.

## About the Project
We utilize [Roboflow](https://roboflow.com/) for annotating and labeling images, ensuring precise and efficient dataset preparation. Our project on Roboflow can be accessed at [Roboboat 2024 Marine Markers Computer Vision Project](https://universe.roboflow.com/icebergasv-ab2fn/roboboat-2024-marine-markers) in [Roboflow Universe](https://universe.roboflow.com/).

This repository contains Jupyter notebooks detailing the training process for the custom dataset. These notebooks are adapted from Roboflow's resources and tailored to our specific requirements for real-world marine marker detection.

The classes in our Custom Dataset include:

- **Black Buoy**
- **Blue Buoy**
- **Green Buoy**
- **Green Marker**
- **Red Buoy**
- **Red Marker**
- **Yellow Buoy**

  ## Project Evolution and Documentation
This repository serves not just as a codebase but also as a living document of our model's evolution. We aim to:

- **Visualize Improvements**: Through our Jupyter notebooks, we provide visual insights into how our model improves over time, showcasing enhancements in detection accuracy and efficiency.
- **Document Changes**: Each stage of our model's development is meticulously documented. This includes changes in training approaches, hyperparameter adjustments, and model architecture modifications.
- **Store Model Weights**: As we progress, we save various iterations of our model's weights. This practice allows us to track improvements and provides options for rollback in case of any regressions.

## Contents
- **Jupyter Notebooks**: Comprehensive guides on training the YOLOv5 model with our custom dataset.
- **Training Weights**: We store the weights of our YOLOv5 models here post-training. These weights are ready for use in object detection tasks or further fine-tuning.

## Training Graphs For Model Evaluation Version ?

### Criteria for Training



## Training Graphs For Model Evaluation Explained
### Loss Graphs
#### Box Loss
- **Ideal Trend**: Steadily decreasing over time.
- **What it Means**: The model is getting better at accurately predicting the bounding boxes around the objects.
#### Object Loss
- **Ideal Trend**: Decreasing over time with potential minor fluctuations.
- **What it Means**: The model is improving its ability to detect objects within the images.
#### Class Loss
- **Ideal Trend**: Decreasing steadily to a low level.
- **What it Means**: The model is becoming more accurate at classifying the objects it has detected.

### Accuracy Graphs
#### Precision
- **Ideal Trend**: Increasing over time.
- **What it Means**: The model is making more true positive predictions compared to false positive predictions, indicating higher accuracy.
#### Recall
- **Ideal Trend**: Increasing over time.
- **What it Means**: The model is correctly identifying a higher proportion of all actual positives, reducing the number of false negatives.
### Mean Average Precision (mAP) Graphs
#### mAP at IoU=0.5
- **Ideal Trend**: Increasing towards 1.
- **What it Means**: The model is accurately detecting objects with an Intersection over Union (IoU) of 0.5, indicating good localization and detection performance.

#### mAP at IoU=0.5:0.95
- **Ideal Trend**: Increasing steadily.
- **What it Means**: The model performs well across a range of IoU thresholds, which is a stringent test of its localization and classification accuracy.

## Interpretation of Trends in Graphs
1. **Overfitting Signs**
If validation loss begins to increase while training loss continues to decrease, the model may be overfitting to the training data and not generalizing well to new data.
2. **Underfitting Signs**
If both training and validation losses are high or not decreasing, the model may be underfitting and not learning the underlying pattern in the data well.
3. **Good Fit Indications**
Training and validation losses decrease and plateau, precision and recall are high, and mAP values are close to 1.
### Notes on Graph Fluctuations
- Fluctuations in graphs are normal but should diminish over time as the model learns.
- Spikes in validation metrics may indicate the presence of outliers or particularly challenging examples in the validation dataset.

## Dataset Annotation and Labelling Documentation
For a comprehensive understanding of our dataset creation, annotation, labelling process, and training methodologies, please refer to our detailed documentation available in our [Gitbook](https://app.gitbook.com/o/vtYvioW5qkBb75Erv7gv/s/OCTt5VIaAFBF4m37LLUi/computer-vision/dataset-creation).
