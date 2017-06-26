# DrawMyOwnNumbers Notebook
A simple notebook for drawing onto a blank canvas so that a user may create their own test samples to input into a trained neural net in Keras. Some code borrowed from Francois Chollet [https://github.com/fchollet](https://github.com/fchollet)

Tkinter is used to provide a canvas for a user to draw on, this is then saved on the hard disk (unfortunately there is not a more elegant method). The saved image is loaded into python and a Gaussian blur is applied. This blurred image is then sampled at a 28*28 grid around the centre of mass and clipped to produce an MNIST stylized version of the original picture.

Information on the Minst images and all the records for various methods can be found here: [http://yann.lecun.com/exdb/mnist/](http://yann.lecun.com/exdb/mnist/)


# Cifar10Converter Notebook
Take an image file, apply a gaussian blur filter and sample to blurred image at a 32*32 grid to get a Cifar10 image.
