### **Colorization of Grayscale CIFAR-10 Images using Deep Learning**

This project demonstrates the colorization of grayscale images from the CIFAR-10 dataset using a deep learning autoencoder. The model is trained to take grayscale input images and reconstruct them in color, providing an efficient approach to image colorization for small-sized datasets like CIFAR-10.

**Project Overview**
The objective is to colorize grayscale versions of CIFAR-10 images by leveraging an autoencoder architecture. The model learns from the color information in the dataset's training images, attempting to map grayscale images to their respective colored versions.

**Dataset**
We use the CIFAR-10 dataset, which contains 60,000 32x32 color images across 10 different classes.

Training Set: 50,000 images
Testing Set: 10,000 images

**Model Architecture**
An autoencoder model is employed to perform image colorization:

- Encoder: Consists of multiple convolutional layers with ReLU activation functions to learn compact representations.
- Decoder: Symmetric convolutional layers with upsampling to reconstruct the color channels.
The output layer has a sigmoid activation function to normalize pixel values between 0 and 1.

**Training**
The model is trained using grayscale images as input and their corresponding RGB images as targets. Training is conducted over 50 epochs with a batch size of 128, using Mean Squared Error as the loss function and Adam optimizer for efficient convergence.

**Installation**
To run this code, follow these steps:
1. Clone the repository:
     ```bash
     git clone git@github.com:ShokufehKhani/Deep-learning-Projects.git
2. Navigate to the project directory:
    ``` bash
    cd colorization-cifar10
3. Install the required dependencies
    ``` bash
    pip install -r requirements.txt

**Usage**
- Load and preprocess the CIFAR-10 data.
- Initialize and compile the autoencoder model.
- Train the model using the training dataset.
- Use the model to colorize grayscale images from the test set.



**Results**
The model successfully colorizes grayscale CIFAR-10 images with reasonable accuracy, producing vibrant reconstructions that reflect the original image colors.

**Sample Output**
Here’s an example of the model’s colorization performance:

- Input: Grayscale image
- Output: Colorized image (Include sample images before and after colorization.)

**Acknowledgments**
CIFAR-10 dataset provided by the Canadian Institute for Advanced Research.
Inspiration from deep learning image colorization research.
