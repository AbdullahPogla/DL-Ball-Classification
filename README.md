This project is a Deep Learning-based Ball Classification system built using PyTorch and a pretrained ResNet18 model. The model classifies 15 different types of sports balls including football, basketball, tennis ball, volleyball, baseball, golf ball, hockey puck, and others. The project applies Transfer Learning to improve performance and reduce training time while using Data Augmentation techniques such as random cropping, horizontal flipping, and color adjustments to improve generalization and reduce overfitting.

The model architecture was modified by replacing the final fully connected layer and adding Dropout regularization. Training was performed using the Adam optimizer with CrossEntropyLoss, while Early Stopping was implemented to prevent overfitting and automatically save the best model based on validation loss. The project also includes visualization of training and testing accuracy/loss curves as well as prediction results showing the true and predicted classes.

The final model achieved approximately 99% training accuracy and around 91% test accuracy, demonstrating strong performance on unseen data. The project is designed to support GPU acceleration using CUDA for faster training and can be extended in the future for real-time camera classification, web deployment, or object detection applications.
Ball Classification using ResNet18

A Deep Learning project for multi-class sports ball classification using Transfer Learning with ResNet18.
The model is trained on a custom dataset containing 15 different ball categories and achieves high classification accuracy using Data Augmentation, Dropout Regularization, and Early Stopping techniques.

Features
Transfer Learning using pretrained ResNet18
Custom dataset with 15 ball classes
Data Augmentation to reduce overfitting
Early Stopping based on validation loss
Automatic best model saving
Training & validation accuracy/loss visualization
Final prediction visualization with true vs predicted labels
GPU support using CUDA
Dataset Classes
American Football
Baseball
Basketball
Billiard Ball
Bowling Ball
Cricket Ball
Football
Golf Ball
Hockey Ball
Hockey Puck
Rugby Ball
Shuttlecock
Table Tennis Ball
Tennis Ball
Volleyball
Technologies Used
Python
PyTorch
Torchvision
Matplotlib
Model Architecture

The project uses:

Pretrained ResNet18
Modified Fully Connected Layer
Dropout Regularization (0.7)
Adam Optimizer
CrossEntropyLoss
Training Techniques
Data Augmentation

The training pipeline includes:

Random Resized Crop
Horizontal Flip
Color Jitter
Image Normalization
Regularization
Dropout
Weight Decay
Early Stopping
Training Results
Training Accuracy reached ~99%
Test Accuracy reached ~91%
Best model saved automatically during training
