
<div align="center">
   <img alt="Logo" src="https://user-images.githubusercontent.com/90816300/174459628-275795d3-8ef7-4248-af3f-6dd82859299a.png" />
</div>

<h1 align="center">
AI Yoga Assistant
</h1>    

This project aims to enhance the yoga experience by utilizing AI to detect and correct yoga poses. The model is trained to recognize various yoga poses and provide real-time feedback on alignment and accuracy, enabling users to improve their practice, reduce injury risk, and ensure correct posture.

## Objective
The goal of this proof of concept (PoC) is to:

- Identify common yoga poses through computer vision.

- Provide feedback on pose alignment and accuracy.

- Suggest adjustments to enhance the user’s practice.

## Use Case

### Pose Detection & Correction:

The application helps users perform yoga poses with accurate alignment by detecting the pose and offering feedback on their posture. The model highlights the misalignment areas and suggests corrective actions. This feature aims to guide yoga practitioners in achieving proper form and prevent common injuries caused by improper posture.

## Dataset

### Data Source: The dataset used for this project is a combination of publicly available datasets such as Yoga-82 Dataset (or any other relevant datasets).
### Dataset Characteristics:
- 82 different yoga poses.

- Images annotated with key landmarks to identify key body points in each pose.

- Multiple angles for each pose.


## Model Development

### Preprocessing
- The images are resized to a fixed size (e.g., 224x224 pixels).

- Keypoint extraction is performed using a pose estimation model (e.g., OpenPose, MediaPipe).

- Data augmentation is applied to improve model robustness and generalization.

## Model Architecture

The model architecture is based on a Convolutional Neural Network (CNN) for pose classification:


- Input Layer: Takes an image or video frame as input.

- Pose Estimation: Uses pose estimation libraries (e.g., OpenPose, MediaPipe) to detect key landmarks (e.g., elbows, knees, hips, etc.).

- Classification Layer: A CNN layer classifies the detected pose into one of the predefined yoga poses.

- Alignment Feedback: A custom-built feedback module compares detected keypoints to the ideal pose and calculates the alignment score.

## Feedback Mechanism
The model generates feedback based on the pose's keypoint alignment.

- A visual overlay shows how far each joint is from the ideal alignment (e.g., angle between joints).

- Suggestions for improving posture are displayed, such as "Keep your shoulders back" or "Straighten your back."

# Website

## Homepage

![homepage](https://user-images.githubusercontent.com/90816300/174463611-3a1c1176-c28d-47ce-bdb8-79ed10ed03c5.png)

## Tracks

![tracks](https://user-images.githubusercontent.com/90816300/174463628-fb45f921-f1ef-4173-b648-1f42c1f454ae.png)

## Yoga

![yoga](https://user-images.githubusercontent.com/90816300/174463632-03670f77-3d97-4fde-8bea-03d8c793d0de.png)

## Livestreaming

![index](https://user-images.githubusercontent.com/90816300/174463641-6c63844a-3f6c-46e5-a7ec-c40ff4dc5048.png)

## Accuracy Chart

![charts](https://user-images.githubusercontent.com/90816300/174463655-e37138f1-1651-4898-85ec-216864a502b9.png)


# Tech Stack Used

## Front-End 

HTML, CSS, JavaScript

## Back-End

Python, Flask, Open CV, Mediapipe, Tensorflow Hub

