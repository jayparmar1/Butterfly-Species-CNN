# 🦋 Butterfly Species Classification (CNN)

This project is a Convolutional Neural Network (CNN) that classifies **40 butterfly species** using TensorFlow and Keras. It includes end-to-end steps: loading data, preprocessing, training, evaluating, and predicting on new images.



## 📦 Dataset
The dataset used is the **Butterfly Images – 40 Species Dataset** (Kaggle).  

The folder structure:
train/
val/
test/


Each subfolder represents a butterfly species.

> ⚠ Dataset is NOT uploaded here due to size.


## 🔧 Data Input Settings

These input parameters were used throughout the project:
Batch Size      = 32
Image Height    = 180
Image Width     = 180

All images are resized to 180 × 180 before feeding into the CNN.


## 🧠 Model Architecture

The model is built using the tf.keras.Sequential API.

# Layers:

* Rescaling(1./255)

* Data Augmentation

  1. Random Horizontal Flip

  2. Random Rotation

  3. Random Zoom

* Convolutional Blocks (3×)

  1. Conv2D → MaxPooling2D

* Dropout(0.2)

* Flatten()

* Dropout(0.5)

* Dense(128, activation='relu')

* Final Dense layer → Output logits for 40 classes


### **Model Summary**
- Input size: 180 × 180 × 3  
- Optimizer: **Adam**  
- Loss: **Sparse Categorical Crossentropy**  
- Best Validation Accuracy: 1. For Train- **80.00%**
                            2. For Val - **76.20%
                            3. For Test- **80.59%  
- Training Epochs: 40 


## 📁 Project Structure

Butterfly-CNN/
│
├── butterfly_cnn.ipynb        # Main training notebook
├── requirements.txt           # Required libraries
├── README.md                  # Project documentation
│
└── sample_images/             # Sample prediction images
       ├── test1.jpg
       ├── test2.jpg
       └── test3.jpg
       └── test4.jpg
       └── test5.jpg
       └── test6.jpg
       
       
## 🛠 Technologies Used

1. Python
2. TensorFlow / Keras
3. NumPy
4. Matplotlib
5. Google Colab / Jupyter Notebook
6. PIL
7. Pathlib
8. os 
9. Google Drive
       
## Thanks 





