# Week-1
This project uses deep learning to classify waste as Organic or Recyclable. A CNN built with TensorFlow and Keras processes images, with OpenCV for preprocessing and Matplotlib for visualization. Data is organized in labeled folders. Run main.py after installing dependencies to preprocess, train, and classify waste efficiently.
## Dataset
The dataset is too large to include in the repository.  
Download it from [Google Drive](https://drive.google.com/file/d/1nQmRpsPgaX-H5B5Ov7CaxPLeqH-9WoZR/view?usp=sharing).  
The dataset comes as a ZIP file. After downloading and extracting the ZIP file, place the files in the following structure:
dataset/
├── TRAIN/
├── TEST/
# Week-2
Week 2 Updates Summary
In Week 2, we have enhanced our deep learning model for waste classification by making significant updates to the Week 1 code. Below are the key improvements and additions:

Data Visualization Enhancement:

Introduced a grid visualization of random images from the dataset using plt.subplot().
The images are randomly selected and labeled, helping us understand dataset variations.
CNN Model Architecture Expansion:

Added a third convolutional layer (128 filters) to capture more complex image features.
Increased model depth to improve accuracy.
Implemented Dropout layers (0.5 rate) in the dense layers to prevent overfitting.
Training and Testing Generators:

Used ImageDataGenerator.flow_from_directory() to dynamically load images from the dataset.
Ensured RGB conversion and maintained 224x224 resolution.
Configured class_mode='categorical' for multi-class classification.
Model Training & Validation:

Trained the model for 10 epochs using the model.fit() function.
Added validation_data=test_generator to track validation performance.
