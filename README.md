** Brain Tumor Detection using CNN**

This project uses Convolutional Neural Networks (CNN) to detect brain tumors from MRI images. It aims to support early diagnosis by automatically classifying MRI scans as either Tumor or Normal, and highlighting the tumor region if detected.

**Dataset**

- Source: https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection
- Structure:
  brain_tumor_dataset/
  ├── Training/
  │   ├── yes/
  │   └── no/
  ├── Testing/
  │   ├── yes/
  │   └── no/
**
 Model Overview**

- Model Type: Convolutional Neural Network (CNN)
- Input Shape: 128x128x3 (resized MRI images)
- Output: Binary classification (Tumor / Normal)
- Libraries: TensorFlow, Keras, OpenCV, NumPy

** Features**

- Binary classification: Detects presence of a brain tumor
- Tumor region is highlighted with a red rectangle
- Clear visual output: Original and Predicted images
- Easily extendable for real-time web or mobile apps

**Installation**

pip install tensorflow opencv-python numpy matplotlib
**
 Project Structure**

brain_tumor_project/
├── train_model.py             # Script to train and save the CNN model
├── model/
│   └── brain_model.h5         # Trained CNN model
├── images/
│   └── predicted.jpg          # Output image with detection
└── utils/
    └── predict_and_draw.py    # Function to predict and annotate tumor

** How to Train the Model**

python train_model.py

Make sure your dataset is correctly placed in the brain_tumor_dataset/ folder.

 **Sample Results**

(Output images with tumor highlighted will be saved in the 'images/' directory.)

 Credits

- Dataset by Navoneel Chakrabarty on Kaggle
- Developed by: Muhammad Hassan Raza

License

This project is for educational and research purposes only.
