# Convolutional Neural Networks (CNNs)

Convolutional Neural Networks (CNNs) are a form of deep learning architecture tailored for image processing and recognition. They employ convolutional layers to extract features from images, followed by pooling layers to reduce dimensionality, and fully connected layers for classification. CNNs are commonly applied in areas such as medical image analysis, object detection, and facial recognition.

## Weight Initialization Techniques

Weight initialization plays a vital role in training deep neural networks, as it affects both the speed of convergence and the model's overall performance. Some commonly used weight initialization methods are:

- **Random Initialization**: Assigning small, random values to the weights.
- **Xavier/Glorot Initialization**: Specifically designed for sigmoid/tanh activation functions.
- **He Initialization**: Suitable for ReLU activation, which reduces the chances of vanishing or exploding gradients.ts.

## Activation Functions

Activation functions add non-linearity to neural networks, allowing them to capture complex patterns. Some commonly used activation functions are:

- **ReLU (Rectified Linear Unit)**: Widely used in CNNs for its ability to efficiently propagate gradients.
- **Tanh**:  Similar to the sigmoid function, but outputs values between -1 and 1, helping to minimize bias shift.
- **Leaky_ReLU**: an activation function where the negative section allows a small gradient instead of being completely zero, helping to reduce the risk of overfitting in neural networks.

## Optimizers

Optimizers change the weights of the network in a way to minimize the loss function. The most commonly used optimizers are:

- **SGD (Stochastic Gradient Descent)**: A simple optimizer with momentum-based updates.
- **Adam (Adaptive Moment Estimation)**: This is the combination of momentum and adaptive learning rates to get a better convergence.
- **RMSprop**: Adjusts learning rates based on the gradient's magnitude, making it ideal for recurrent networks.

## ResNet (Residual Networks)

ResNet-18 is a deep convolutional network developed to address the vanishing gradient issue through skip connections (residual learning). This architecture allows for the training of very deep networks without a drop in performance, making it particularly effective for image classification tasks.

## Tabulated Results for Different Combinations

| Configuration | Activation Function | Weight Initialization | Optimizer | Accuracy | Loss |
| ------------- | ------------------- | --------------------- | --------- | -------- | ---- |
| 1             | ReLU                | Xavier                | SGD       | 51.01    | 0.70 |
| 2             | ReLU                | Xavier                | Adam      | 49.72    | 0.66 |
| 3             | ReLU                | Xavier                | RMSprop   | 52.95    | 0.65 |
| 4             | ReLU                | Kaiming               | SGD       | 49.78    | 0.75 |
| 5             | ReLU                | Kaiming               | Adam      | 61.30    | 0.62 |
| 6             | ReLU                | Kaiming               | RMSprop   | 51.74    | 0.68 |
| 7             | ReLU                | Random                | SGD       | 47.78    | 0.69 |
| 8             | ReLU                | Random                | Adam      | 56.63    | 0.69 |
| 9             | ReLU                | Random                | RMSprop   | 55.34    | 0.72 |
| 10            | Tanh             | Xavier                | SGD       | 50.78    | 0.71 |
| 11            | Tanh             | Xavier                | Adam      | 55.62    | 0.63 |
| 12            | Tanh             | Xavier                | RMSprop   | 48.78    | 0.70 |
| 13            | Tanh             | Kaiming               | SGD       | 52.73    | 0.69 |
| 14            | Tanh             | Kaiming               | Adam      | 58.62    | 0.69 |
| 15            | Tanh             | Kaiming               | RMSprop   | 50.78    | 0.70 |
| 16            | Tanh             | Random                | SGD       | 51.74    | 0.67 |
| 17            | Tanh             | Random                | Adam      | 57.65    | 0.68 |
| 18            | Tanh             | Random                | RMSprop   | 48.78    | 0.66 |
| 19            | Leaky_ReLU                | Xavier                | SGD       | 52.78    | 0.65 |
| 20            | Leaky_ReLU                | Xavier                | Adam      | 55.64    | 0.69 |
| 21            | Leaky_ReLU                | Xavier                | RMSprop   | 49.72    | 0.64 |
| 22            | Leaky_ReLU                | Kaiming               | SGD       | 51.70    | 0.71 |
| 23            | Leaky_ReLU                | Kaiming               | Adam      | 56.64    | 0.63 |
| 24            | Leaky_ReLU                | Kaiming               | RMSprop   | 48.79    | 0.69 |
| 25            | Leaky_ReLU                | Random                | SGD       | 52.77    | 0.65 |
| 26            | Leaky_ReLU                | Random                | Adam      | 55.62    | 0.69 |
| 27            | Leaky_ReLU                | Random                | RMSprop   | 50.75    | 0.70 |

**Best-Performing Model**: Based on accuracy and loss, the best configuration consists of the **ReLU** activation function, **Kaiming** weight initialization, and the **Adam** optimizer.

# Conclusions

- The different combinations of activation function, weight initialization, and optimizer significantly is important CNN Model analysis.
- Based on accuracy and loss, the best configuration consists of the **ReLU** activation function, **Kaiming** weight initialization, and the **Adam** optimizer.
- ResNet-10 performz better in classification analysis.

-


