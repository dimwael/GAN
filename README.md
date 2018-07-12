# GAN
Generative Adversarial Networks to create Fake real images

GANs — originally proposed by Ian Goodfellow — have two networks, a *generator* and a *discriminator*. They are both trained at the same time and compete again each other in a minimax game. The generator is trained to fool the discriminator creating realistic images, and the discriminator is trained not to be fooled by the generator.

GAN training overview GAN training overview.

At first, the generator generates images. It does this by sampling a vector noise Z from a simple distribution (e.g. normal) and then upsampling this vector up to an image. In the first iterations, these images will look very noisy. Then, the discriminator is given fake and real images and learns to distinguish them. The generator later receives the “feedback” of the discriminator through a backpropagation step, becoming better at generating images. At the end, we want that the distribution of fake images is as close as possible to the distribution of real images. Or, in simple words, we want fake images to look as plausible as possible.

It is worth mentioning that due to the minimax optimization used in GANs, the training might be quite unstable. There are some hacks, though, that you can use for a more robust training.

![Image](http://guimperarnau.com/files/blog/Fantastic-GANs-and-where-to-find-them/GAN_training_overview.jpg)

- The Generator part :
![image](https://cdn-images-1.medium.com/max/2000/1*UKStYTQdgoQYVp_ynNIaLA.png)

# Results : 
Images produced after many hours of traininig :
-First Created Image :
![alt text](https://github.com/dimwael/GAN/blob/master/results/fake_samples_epoch_001.png)
- Latest Images (10 & 11)

![alt text](https://github.com/dimwael/GAN/blob/master/results/fake_samples_epoch_010.png)
![alt text](https://github.com/dimwael/GAN/blob/master/results/fake_samples_epoch_011.png)
