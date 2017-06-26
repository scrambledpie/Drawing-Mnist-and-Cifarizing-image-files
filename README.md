# DrawMyOwnNumbers Notebook
A simple notebook for drawing onto a blank canvas so that a user may create their own test samples to input into a trained neural net in Keras. Some code borrowed from Francois Chollet [https://github.com/fchollet](https://github.com/fchollet)

Tkinter is used to provide a canvas for a user to draw on, this is then saved on the hard disk (unfortunately there is not a more elegant method). The saved image is loaded into python and a Gaussian blur is applied. This blurred image is then sampled at a 28*28 grid around the centre of mass and clipped to produce an MNIST stylized version of the original picture.

Information on the Minst images and all the records for various methods can be found here: [http://yann.lecun.com/exdb/mnist/](http://yann.lecun.com/exdb/mnist/)

---

# Cifar10Converter Notebook
The Cifar10 Dataset is a collection of 50,000 train + 10,000 test images from 10 classes, ranging from cats to aeroplanes. more info can be found at [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html).

This notebook contains a funciton that takes an image file and a set of cropping boundaries, applies a gaussian blur filter and samples the blurred image at a 32*32 grid evenly spaced within the boundaries to get a Cifar10 image ready to be fed into whatever keras model you like!
