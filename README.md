# Generation-Of-Synthetic-Images-With-DCGANs-In-Keras-From-Fashion-MNIST-Dataset
Generation Of Synthetic Images From Fashion MNIST Dataset With DCGANs In Keras.


Generative Adversarial Networks (GANs) are one of the most interesting ideas in computer science today. Two models are trained simultaneously by an adversarial process. A generator ("the artist") learns to create images that look real, while a discriminator ("the art critic") learns to tell real images apart from fakes.


During training, the generator progressively becomes better at creating images that look real, while the discriminator becomes better at telling them apart. The process reaches equilibrium when the discriminator can no longer distinguish real images from fakes.

DCGAN is one of the popular and successful network design for GAN. It mainly composes of convolution layers without max pooling or fully connected layers. It uses convolutional stride and transposed convolution for the downsampling and the upsampling.


A DCGAN is a direct extension of the GAN described above, except that it explicitly uses convolutional and convolutional-transpose layers in the discriminator and generator, respectively. It was first described by Radford et. al. in the paper Unsupervised Representation Learning With Deep Convolutional Generative Adversarial Networks. The discriminator is made up of strided convolution layers, batch norm layers, and LeakyReLU activations. The input is a 3x64x64 input image and the output is a scalar probability that the input is from the real data distribution. The generator is comprised of convolutional-transpose layers, batch norm layers, and ReLU activations. The input is a latent vector, z, that is drawn from a standard normal distribution and the output is a 3x64x64 RGB image. The strided conv-transpose layers allow the latent vector to be transformed into a volume with the same shape as an image.


Summary of DCGAN:
  1. Replace all max pooling with convolutional stride
  2. Use transposed convolution for upsampling.
  3. Eliminate fully connected layers.
  4.Use Batch normalization except the output layer for the generator and the input layer of the discriminator.
  5. Use ReLU in the generator except for the output which uses tanh.
  6. Use LeakyReLU in the discriminator.
  

Technology: Deep Convolutional Generative Adversarial Network (DCGAN) | Python | Tensorflow 2.0 | Keras | MNIST Dataset | Artificial Neural Networks | Machine Learning | Deep Learing | Neural Networks | Artificial Intelligence
