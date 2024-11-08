### **Realistic Human Face Generation with GANs**

This project implements a Generative Adversarial Network (GAN) to generate realistic human face images using the CelebA dataset. The model trains a deep convolutional GAN architecture to create synthetic faces by learning from real celebrity images in CelebA. This project utilizes a TensorFlow/Keras-based model with GPU acceleration for faster training.

### **Key Features**
- **Dataset**: Uses the CelebA dataset, a large-scale collection of celebrity faces, for training.
- **Model Architecture**: Builds a GAN with a generator and a discriminator to generate high-quality, realistic face images.
- **Training Process**:
- Discriminator trains to distinguish real images from generated ones.
- Generator learns to produce images that are indistinguishable from real faces.
- **Visualization**: Displays generated faces every 5 epochs and plots generator and discriminator loss over time to monitor training.

**Installation and Setup**
1. Clone the repository:
  ```bash
  git clone https://github.com/ShokufehKhani/Deep-learning-Projects.git

2. Navigate to project directory
  ```bash
  cd "Generating Realistic Human Faces with GANs: A Deep Learning Approach"

2. Install required libraries:
  ```bash
  pip install -r requirements.txt
