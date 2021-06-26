# How to Configure Image Data Augmentation in Keras.
<p align="center">
  <img width="512" height="512" src="https://github.com/ChitralwarManik/Data-Augmentation-/blob/main/New%20task/Augmented%20Images/data-set-icon-11.jpg">
</p>

# What is Data Augmentation ?

Image data augmentation is a technique that can be used to artificially expand the size of a training dataset by creating modified versions of images in the dataset.

Training deep learning neural network models on more data can result in more skillful models, and the augmentation techniques can create variations of the images that can improve the ability of the fit models to generalize what they have learned to new images.

The Keras deep learning neural network library provides the capability to fit models using image data augmentation via the ImageDataGenerator class.

* Image data augmentation is used to expand the training dataset in order to improve the performance and ability of the model to generalize.
* Image data augmentation is supported in the Keras deep learning library via the ImageDataGenerator class.
* How to use shift, flip, brightness, and zoom image data augmentation.

![]https://github.com/ChitralwarManik/Data-Augmentation-/blob/main/New%20task/Augmented%20Images/data-set-icon-11.jpg)

The performance of deep learning neural networks often improves with the amount of data available.

Data augmentation is a technique to artificially create new training data from existing training data. This is done by applying domain-specific techniques to examples from the training data that create new and different training examples.

Image data augmentation is perhaps the most well-known type of data augmentation and involves creating transformed versions of images in the training dataset that belong to the same class as the original image.

Transforms include a range of operations from the field of image manipulation, such as shifts, flips, zooms, and much more.

The intent is to expand the training dataset with new, plausible examples. This means, variations of the training set images that are likely to be seen by the model. For example, a horizontal flip of a picture of a cat may make sense, because the photo could have been taken from the left or right. A vertical flip of the photo of a cat does not make sense and would probably not be appropriate given that the model is very unlikely to see a photo of an upside down cat.

As such, it is clear that the choice of the specific data augmentation techniques used for a training dataset must be chosen carefully and within the context of the training dataset and knowledge of the problem domain. In addition, it can be useful to experiment with data augmentation methods in isolation and in concert to see if they result in a measurable improvement to model performance, perhaps with a small prototype dataset, model, and training run.

Modern deep learning algorithms, such as the convolutional neural network, or CNN, can learn features that are invariant to their location in the image. Nevertheless, augmentation can further aid in this transform invariant approach to learning and can aid the model in learning features that are also invariant to transforms such as left-to-right to top-to-bottom ordering, light levels in photographs, and more.

Image data augmentation is typically only applied to the training dataset, and not to the validation or test dataset. This is different from data preparation such as image resizing and pixel scaling; they must be performed consistently across all datasets that interact with the model.

# Image Augmentation With ImageDataGenerator
The Keras deep learning library provides the ability to use data augmentation automatically when training a model.

This is achieved by using the ImageDataGenerator class.

First, the class may be instantiated and the configuration for the types of data augmentation are specified by arguments to the class constructor.

A range of techniques are supported, as well as pixel scaling methods. We will focus on five main types of data augmentation techniques for image data; specifically:

* Image shifts via the `width_shift_range` and `height_shift_range`` arguments.
* Image flips via the `horizontal_flip` and `vertical_flip` arguments.
* Image rotations via the `rotation_range argument
* Image brightness via the `brightness_range` argument.
* Image zoom via the `zoom_range` argument.

# Original Images
![](https://github.com/ChitralwarManik/Data-Augmentation-/blob/main/New%20task/images/cat.jpg)

![](https://github.com/ChitralwarManik/Data-Augmentation-/blob/main/New%20task/images/face.jpg)

# Augmented Images
![](https://github.com/ChitralwarManik/Data-Augmentation-/blob/main/New%20task/Augmented%20Images/Capture.PNG)
![](https://github.com/ChitralwarManik/Data-Augmentation-/blob/main/New%20task/Augmented%20Images/Capture1.PNG)

Thanks
