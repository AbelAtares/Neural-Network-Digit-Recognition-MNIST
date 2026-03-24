# Handwritten Digit Recognition with a Neural Network

This project explores the MNIST dataset to recognize handwritten digits (0–9) using a small neural network implemented from scratch in NumPy. The goal is to demonstrate how a simple network can learn from raw data and make accurate predictions.

---

## 1. Import and Study Data
- The dataset is loaded from a CSV file called train.csv.
- It contains 42,000 images, each representing a digit from 0 to 9.
- Each image has 784 pixels, with values ranging from 0 (black) to 255 (white).
- This step allows us to understand the structure and scale of the dataset before training the model.
## 2. Data Split
- The dataset is split into Training and Development sets:
- Development Set: 1,000 records
- Training Set: 41,000 records
- This ensures we can train the model on most of the data while keeping a small portion to validate performance.
## 3. Model Implementation
- The neural network architecture consists of:
- Input Layer: 784 neurons (one per pixel)
- Hidden Layer: 10 neurons with ReLU activation function
- Output Layer: 10 neurons with Softmax activation function
- In this section, we also define:
- Forward Propagation: to calculate predictions
- Backward Propagation: to compute gradients and update the weights and biases
## 4. Model Training
- The network is trained using Gradient Descent.
- During training, weights and biases are iteratively updated to minimize the loss.
- After 600 iterations, the model reaches an accuracy of approximately 88%, demonstrating effective learning from the data.
## 5. Model Testing
- The Test Prediction function is used to:
- Select individual images from the dataset
- Compare the predicted label with the actual value
- Visualize the image alongside its prediction
- This provides a clear understanding of how well the model performs on unseen examples.
## Conclusion
- Even with a relatively small neural network, we achieve very good accuracy (~88%) on MNIST.
- This project demonstrates the power of gradient descent, forward/backward propagation, and neural networks from scratch, making it a solid educational example for understanding the fundamentals of deep learning.
