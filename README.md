Multilabel Image Classification 

This project implements a deep learning based multilabel classification system for fashion images.

Approach:
- Used pretrained ResNet18 (ImageNet weights)
- Modified final layer for 4 attribute prediction
- Applied sigmoid activation for multilabel outputs
- Implemented masked binary cross entropy to handle missing labels (NA)
- Handled missing images during data loading
- Fine-tuned the model on provided dataset

Training:
- Batch size: 16
- Optimizer: Adam
- Learning rate: 1e-4
- Epochs: 5
- Loss curve plotted and saved

Inference:
- Model predicts attributes present in an input image using sigmoid thresholding.

Additional Improvements:
- GPU training
- Robust dataset loader
- Handling dataset imbalance via masked loss
