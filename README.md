**Autoencoder for Google Quick Draw Dataset**
**Overview**
This project implements an autoencoder model trained on a subset of the Google Quick Draw dataset. The dataset consists of 50 million drawings across 345 categories, making it a great alternative to MNIST for exploring computer vision tasks.
The model is built using TensorFlow and Keras, and consists of an encoder, decoder, and the complete autoencoder network. The architecture is based on convolutional layers, designed to compress the input image into a smaller latent representation and then reconstruct it back to its original form.

**Dataset**
The dataset used is a simplified version of the Google Quick Draw dataset. Each drawing is represented as a 28x28 grayscale image.

**Model Architecture**
The model consists of three parts:
1. Encoder
Three convolutional layers with ReLU activation
Max pooling layers to downsample the image
2. Decoder
Three convolutional layers with ReLU activation
UpSampling layers to restore the original image size
Final convolutional layer with Sigmoid activation to produce the output
3. Autoencoder
Combines encoder and decoder into one end-to-end network
Compiled with Adam optimizer and Binary Crossentropy loss function
Files
autoencoder_model.py: Contains the full implementation of the autoencoder, encoder, and decoder.


This file — explains the project.
Setup and Installation
Clone the repository:
**Install dependencies:** pip install tensorflow numpy matplotlib

**Run the script:**
autoencoder.ipynb

**Usage**

The autoencoder is trained to compress and reconstruct images.
The encoder extracts latent representations (compressed versions).
The decoder reconstructs images from the latent representation.

**Output**
The model outputs:
Reconstructed images — to visualize how well the autoencoder learns the dataset
Encoded representations — low-dimensional embeddings useful for clustering or other tasks

**Future Improvements**
Add dropout or batch normalization for better performance
Implement training on the full Quick Draw dataset
Explore different architectures like Variational Autoencoders (VAEs)

**Credits**
Dataset: Google Quick Draw Dataset
TensorFlow/Keras for the deep learning framework

Happy coding! 🚀

