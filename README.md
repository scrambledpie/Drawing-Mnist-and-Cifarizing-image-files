# Mnist-drawing-with-Keras
A simple notebook for drawing onto a blank canvas for a user to create their own test samples for a  trained neural net in Keras.

Tkinter is used to draw provide a canvas for a user to draw on, this is then saved on the hard disk (unfortunately there is not a more elegant method). The saved image is loaded into python and a Gaussian blur is applied. This blurred image is then sampled at a 28*28 grid around the centre of mass and clipped to produce an MNIST stylized version of the original picture.

Information on the Minst images and all the records for various methods can be found here: [http://yann.lecun.com/exdb/mnist/](http://yann.lecun.com/exdb/mnist/)
