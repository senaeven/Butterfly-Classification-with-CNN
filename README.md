# Butterfly-Classification-with-CNN
This project focuses on classifying 75 different butterfly species using a Convolutional Neural Network (CNN).

## Features 
- The dataset contains 75 butterfly classes.  
- Images are preprocessed and augmented to improve model generalization.  
- The CNN architecture consists of **3 convolutional layers**, each followed by a **max pooling layer**, designed to extract hierarchical features.  
- The model is trained for **50 epochs** using various **optimizers** (Adam, SGD, RMSprop) and **learning rates** to find the best configuration.  
- Training and validation performance is visualized to monitor accuracy and loss over epochs.  

## Goal 
The aim is to enable automatic recognition of butterfly species, contributing to biodiversity studies and practical applications in computer vision.

## Metrics
The CNN model was evaluated using **training and validation accuracy**. The main findings are:  

- **Adam (lr=0.001)** achieved the best performance, reaching **72.67% training accuracy** and **70.08% validation accuracy**.  
- **Adam (lr=0.01)** completely failed to learn, indicating divergence due to too high a learning rate.  
- **SGD (lr=0.01)** performed reasonably well, with **67.37% training accuracy** and **64.61% validation accuracy**.  
- **RMSprop (lr=0.01)** showed weak learning, producing much lower accuracies compared to other optimizers.  
Overall, **Adam with lr=0.001** proved to be the most effective choice for this dataset and CNN architecture.  
The **confusion matrix** shows that most classes were correctly classified, with only a few misclassifications spread across classes.  
The **accuracy and loss plots** per epoch demonstrate stable convergence, with training and validation curves showing minimal overfitting.  
These results highlight that careful selection of **optimizers and learning rates** is critical for good performance, and that the **3 convolutional + 3 pooling layer CNN** can successfully learn meaningful features from butterfly images.

## Future Directions
This project provides a foundation for butterfly species classification and can be further enhanced in the future. For example, real-time classification could allow identification from live images, dynamic dataset expansion could improve the model’s adaptability to new species, and a user-friendly web or mobile interface could make it accessible to non-technical users. 
This project also strengthens my skills in deep learning, computer vision, and data science, supporting my career growth in AI and environmental applications.

## Links
https://www.kaggle.com/code/senaeven/butterfly-classification-with-cnn
