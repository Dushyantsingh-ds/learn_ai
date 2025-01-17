# Mask Detection AI from Scratch

This project involves creating a mask detection AI from scratch without using any external libraries. The goal is to detect whether a person is wearing a mask or not in an image.

---

## Steps to Build the Project

### 1. Understand the Problem
- **Define the Goal**: Detect whether a person is wearing a mask or not in an image.
- **Input and Output**:  
  - Input: An image.  
  - Output: Binary classification (mask/no mask).

---

### 2. Prepare Your Data
- **Dataset Creation**: Collect images of people with and without masks. ->https://www.kaggle.com/datasets/omkargurav/face-mask-dataset
- **Preprocessing**: Write your own functions for:
  - Image loading
  - Resizing
  - Normalization
- **Data Splitting**: Manually split the data into:
  - Training set
  - Validation set
  - Test set

---

### 3. Design the Neural Network
- **Implement a Basic Neural Network**:
  - Write functions for:
    - Matrix multiplications
    - Activation functions (e.g., sigmoid, ReLU)
    - Forward propagation
  - Define the layers manually.
- **Backpropagation**:
  - Write derivatives and update rules for weights and biases.
  - Implement optimization algorithms like gradient descent.

---

### 4. Implement Training Pipeline
- **Loss Function**: Write a binary cross-entropy loss function from scratch.
- **Batch Processing**: Create a loop to feed batches of images to the network.
- **Weight Updates**: Update weights using gradients from backpropagation.
- **Epochs**: Loop through the dataset multiple times while tracking:
  - Loss
  - Accuracy

---

### 5. Testing and Validation
- Evaluate the model using the test set.
- Write a function to calculate metrics such as:
  - Precision
  - Recall
  - F1-score

---

### 6. Mask Detection Logic
- **Face Detection**:
  - Integrate a custom object detection mechanism to crop faces from images.
  - Use a sliding window approach for face detection.
- **Classification**:
  - Implement logic to classify whether a person is wearing a mask.

---

### 7. Real-Time Implementation (Optional)
- Capture live video using hardware interfacing (e.g., OpenCV if allowed).
- Process video frames in real-time through the detection pipeline.

---

### 8. Optimization
- Fine-tune the model by:
  - Adjusting learning rates
  - Adding more training data
  - Modifying the network structure

---

### 9. Testing and Refinement
- Test various cases to ensure the model generalizes well.
- Address potential errors:
  - False positives
  - False negatives

---

## Tools Developed Manually
- **Image Processing**:
  - Functions for grayscale conversion, resizing, and normalization.
- **Neural Network**:
  - Complete implementation for training and inference.
- **Face Detection**:
  - Basic detection mechanism.
- **Mask Detection**:
  - Classification logic for mask/no mask detection.

---

### Note
This project is implemented **without using external libraries** to fully understand the underlying concepts of machine learning and neural networks.
