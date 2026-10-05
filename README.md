# Pet Face Classification using ResNet50



A deep learning image classification project that identifies pet breeds/categories from images using **ResNet50 transfer learning**.



#### **Overview**



This project focuses on classifying pet images into \*\*16 different cat and dog breed categories\*\* using a deep learning image classification model.



A **ResNet50 model pretrained on ImageNet** is used as a feature extractor. Its pretrained convolutional layers are kept frozen, while a custom classification layer is trained for the target pet categories.



The project demonstrates an end-to-end computer vision workflow, from image preprocessing and dataset preparation to model training, evaluation, and visual prediction analysis.



#### **Objective**



The objective is to build a multiclass image classification model capable of identifying the breed/category represented in a pet image.



#### **Model Approach**



The project uses **transfer learning** instead of training a convolutional neural network from scratch.



The approach consists of:



* ResNet50 pretrained on ImageNet
* Frozen pretrained convolutional layers
* Data augmentation using random flipping and rotation
* A custom classification head with a softmax output layer
* 10 epochs of model training



The final model predicts one of 16 pet categories.



#### **Project Workflow**



Pet Images

&#x20;   ↓

Image Loading

&#x20;   ↓

Label Extraction from Filenames

&#x20;   ↓

Image Resizing and Padding

&#x20;   ↓

Label Encoding

&#x20;   ↓

Train / Validation / Test Split

&#x20;   ↓

Data Augmentation

&#x20;   ↓

ResNet50 Feature Extraction

&#x20;   ↓

Custom Classification Layer

&#x20;   ↓

Model Training

&#x20;   ↓

Model Evaluation

&#x20;   ↓

Prediction Analysis



#### **Technologies Used**



* Python
* TensorFlow
* Keras
* ResNet50
* NumPy
* Pandas
* Matplotlib
* Scikit-learn



#### **Dataset**



The project uses a collection of pet images belonging to 16 categories, including both cat and dog breeds. The image filenames contain the corresponding breed/category information, which is extracted during preprocessing and converted into numerical class labels. **The dataset is not included in this repository**.



#### **Results**



| **Metric**            |                             **Result** |

| ----------------- | ---------------------------------- |

| Test Accuracy     |                             92.03% |

| Test Loss         |                             0.2458 |

| Number of Classes |                                 16 |

| Training Epochs   |                         	      10 |

| Backbone          |      ResNet50 (ImageNet pretrained)|



#### **Evaluation**



Model performance was analyzed using:

* Test accuracy and loss
* Classification report
* Confusion matrix
* Sample predictions
* Correctly classified examples
* Incorrectly classified examples



These evaluations provide both quantitative and visual insights into the model's performance across the 16 pet categories.



#### **Project Structure**



Pet-Face-Classification-Using-ResNet50/

│

├── Pet\_faces.ipynb

├── README.md

└── .gitignore



#### **How to Run**



1. ###### Clone the Repository



git clone https://github.com/Apurva238/Pet-Face-Classification-Using-ResNet50.git

cd Pet-Face-Classification-Using-ResNet50



###### 2\. Prepare the dataset



Create an images/ directory in the project folder and place the required .jpg images inside it.

The notebook expects the following structure:

Pet-Face-Classification-Using-ResNet50/

│

├── Pet\_faces.ipynb

├── images/

│   ├── image1.jpg

│   ├── image2.jpg

│   └── ...

└── README.md



###### 3\. Open the notebook



jupyter notebook Pet\_faces.ipynb



###### 4\. Run the notebook



Execute the cells from top to bottom to perform preprocessing, training, evaluation, and prediction analysis.



#### **Key Takeaway**



This project demonstrates how transfer learning with a pretrained ResNet50 model can be applied to multiclass pet image classification. By reusing features learned from ImageNet and training a task-specific classification layer, the model achieved 92.03% test accuracy on the selected 16-category pet dataset.



#### **Project Context**



This project was developed as part of my AI internship at 1Stop and provided hands-on experience with deep learning, computer vision, transfer learning, image preprocessing, model evaluation, and prediction analysis





























