# Digit-Recognition

The MNIST dataset comprises 60,000 training and 10,000 testing handwritten digits, aiding various image processing systems. Each image, sized 28x28 pixels, was collected from Census Bureau employees and high school students, offering a rich resource for testing diverse methods.

![Image](Pink Black Photocentric Neon Tech Talk Podcast Instagram Post.png)




## Setup:

As with the last project, please use Python's NumPy numerical library for handling arrays and array operations; use matplotlib for producing figures and plots.

This project will be split into two parts. Project 2 (this project) consists of the first part, and Project 3 will cover the second part.

**Note on software:** For all the projects, we will use Python 3.6 augmented with the NumPy numerical toolbox, the matplotlib plotting toolbox. In this project, we will also use the scikit-learn package, which you could install in the same way you installed other packages, by `conda install scikit-learn` or `pip install sklearn`.

1. Download the project and untar it into a working directory. The archive contains various data files in the `Dataset` directory, along with the following Python files:

   - `part1/linear_regression.py`: where you will implement linear regression
   - `part1/svm.py`: where you will implement support vector machine
   - `part1/softmax.py`: where you will implement multinomial regression
   - `part1/features.py`: where you will implement principal component analysis (PCA) dimensionality reduction
   - `part1/kernel.py`: where you will implement polynomial and Gaussian RBF kernels
   - `part1/main.py`: where you will use the code you write for this part of the project

2. To get warmed up to the MNIST dataset, run `python main.py`. This file provides code that reads the data from `mnist.pkl.gz` by calling the function `get_MNIST_data` provided for you in `utils.py`. The call to `get_MNIST_data` returns NumPy arrays:

   - `train_x`: A matrix of the training data. Each row of `train_x` contains the features of one image, which are simply the raw pixel values flattened out into a vector of 
      length. The pixel values are float values between 0 and 1 (0 stands for black, 1 for white, and various shades of gray in-between).
   - `train_y`: The labels for each training datapoint, also known as the digit shown in the corresponding image (a number between 0-9).
   - `test_x`: A matrix of the test data, formatted like `train_x`.
   - `test_y`: The labels for the test data, which should only be used to evaluate the accuracy of different classifiers in your report.

3. Next, we call the function `plot_images` to display the first 20 images of the training set. Look at these images and get a feel for the data (don't include these in your write-up).
