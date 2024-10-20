# Physics Informed Machine Learning
This respository contains all projects pertaining to the course Neural Network Methods for Signals in Engineering, taken at the University of Washington. The course provides an introduction to PyTorch, and the lab materials are paired with lectures from the corresponding week of the course.

## List of Projects:
- ### Data Preparation for ML
  Provides an overview of how data preprocessing is conducted for neural network training.
- ### Iris Classification with Regression
  Uses the Iris datasets to perform simple regression.
- ### MNIST Classification with FCN
  A simple fullly connected NN for classifying hand writted digits in the MNIST dataset.
- ### Fashion MNIST Classificaion
  A simple CNN for classifying fashion in the MNIST fashion dataset.
- ### Create Arthur Conan Doyle AI with RNN
  RNN architecture for generating sentence sequences similar to Sherlock Holmes.
- ### Stock Prediction AI with Encoder-Decoder RNN
  Encoder-Decoder RNN architecture for predicting the next 100 days of stock values, using data from companies including Google, Tesla, and DJI.
- ### German to English Translation with Attention-Mechanism Transformer Model
  Sequence-to-Sequence Transformer model for translating German sentences into English.
- ### Final Project: Generating Stellar Images with Convolutional Autoencoder
  We had freedom to choose our final project, and I was most intrigued by image generation. Project proposes a convolutional autoencoder for determining the image of stellar spectra, attempting to investigate the relation between stellar spectra and image.

## Tools:
  - Python
  - PyTorch
  - Scikit Learn
  - Requests (for data retrieval)

## Results of Final Project
Our convolutional autoencoder is able to generate images of stellar spectra with over 85% accuracy. We focused on the galaxy class to achieve our goals in the provided time frame, and visualizations of the results are below:

![Best image predictions of convolutional autoencoder](https://github.com/mmlegate/Physics-Informed-ML/blob/main/auto_cnn_best.webp?raw=true)  ![Worst image predictions of convolutional autoencoder](https://github.com/mmlegate/Physics-Informed-ML/blob/main/auto_cnn_worst.webp?raw=true)

Plot of Spectra and Image Performance, using SSIM Index
![Pairplot of spectra data and performance](https://github.com/mmlegate/Physics-Informed-ML/blob/main/auto_cnn_pairplot.webp?raw=true)

We see that the original spectra data shows a roughly a linear relationship between two values, as values increase, the data points disperse and show greater variation. Lighter colors in the pairplot above indicate better performance, or a better SSIM index. Also notice the dispersion of redshift values, which is most significant to our spectrum of visible light and thus pivotal to image generation. Most notably, low redshift values corresponding to high z, i, r, g, u values is where the neural network performed the worst. 

