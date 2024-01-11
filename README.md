# PotatoPathoID
## Introduction

Potato (*Solanum tuberosum*) is the fourth-most important staple crop globally. This project identifies and classifies major potato diseases for targeted treatments, aiming to reduce excessive pesticide use.

## Problem Statement

Potato crops are highly vulnerable to diseases, impacting yield and food security. Traditional diagnosis methods are slow, urging the need for automated, scalable solutions.

## Methodology

### Dataset Preparation

Utilized the 'PlantVillage' dataset, including 1000 images each of 'Early Blight' and 'Late Blight', and 152 'Healthy' leaf images, totaling 2152 potato leaf images.
![image](https://github.com/PG-Zen01/PotatoPathoID/assets/156335467/0425f364-308d-4910-8bf7-f82f93cb77f9)


### Data Preprocessing

- Batch Loading: Organized into 68 batches of 32 images each.
- Data Resizing: Standardized to 256 x 256 pixels.
- Data Augmentation: Implemented random flipping and rotation.

### Model Building

- CNN Model Architecture: 6 convolutional layers, 6 max-pooling layers, a dropout layer, and 2 dense layers.
- Model Compilation: Used Adam optimizer, Sparse categorical cross-entropy loss, and Accuracy metric.
- Training Process: 50 epochs, each comprising 54 steps.

### FastAPI Integration

- Endpoint Creation: Developed a FastAPI server on localhost, port 8000.
- Endpoint Routes: Implemented '/predict' for image processing and model prediction.
- ![image](https://github.com/PG-Zen01/PotatoPathoID/assets/156335467/90e223bf-8b75-4b80-baca-0d246955f367)


## Result

The model achieved a remarkable 98.83% test accuracy in classifying potato leaves into three categories: early blight, late blight, and healthy conditions.
![image](https://github.com/PG-Zen01/PotatoPathoID/assets/156335467/8a085227-235a-46fa-b1c6-e1b67c70424a)


## Conclusion

- Robust Data Preparation: Enhanced dataset quality and diversity.
- Impressive Model Accuracy: Demonstrates deep learning's effectiveness in disease classification.
- User-Friendly Implementation: Empowers farmers and experts for on-the-spot diagnosis.

---
