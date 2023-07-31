# Dataset Preprocessing

A good dataset is a key for successful model training. This assignment guides you on how to create two labeled datasets, which could later be used for supervised learning.

## Overview

Image augmentations are used to increase the variability and robustness of a dataset. 
The goal of this assignment is to create a larger dataset from a smaller one.

## Goals

1. The original MNIST dataset includes images of single digits, in ten classes. Your goal is to create a new three-digit image dataset, with 101 classes, based on the original MNIST dataset.
2. Create a dataset of shape images with three classes: Triangle, Rectangle, and Circle/Elipse.

## Tasks

### Task 1 - MNIST
1. Show at least 5 samples of each class (0-9). Always add proper titles and choose the correct color map.
2. Your new dataset should include the three-digits numbers: [000, 001, ..., 055, ..., 099, 100], forming 101 classes. 
3. Each class should have at least 4000 different samples: Use the augmentations you created on lab 3 on your new dataset and show some results. Explain which augmentations are applicable to this specific dataset, which are not, and why.
4. Display typical results of your dataset, demonstrating the variability of the new dataset.
5. Write a detailed summary of your work.

### Task 2 - Shapes Dataset
Shapes definition and functions requirements:

1. Minimal and maximal area: 100-600 pixels, the shape could not be cropped by image boundaries.
2. Each shape will have random size, location, orientation, and color.
3. Each image will include one of the following shapes: Triangle, Rectangle, Circle/Elipse.
4. Each image should be of dimensions 50x50x3.
5. Create at least 300 different samples of each class i.e.(circles with different radius, etc..)

Show the images you created without augmentations and with the augmentations from lab 3.
Write a class, which loads the data you created, labels the data, i.e (triangle will be class 0, rectangle 1, etc.. an Integer) and splits it to train and test sets. 90% of the data should be train images and 10% test images.
