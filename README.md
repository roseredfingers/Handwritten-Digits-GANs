# Handwritten-Digits-GANs
This model generates handwritten digits using GANs using the Handwritten Digits MNIST Dataset.

Generative Adversarial Networks (GANs) train generative models using supervised learning using two sub-models: a Generator and a Discriminator. The Generator creates fake images based on the dataset whereas the Discriminator, on the other hand, classifies the generated images as real or fake. The task of the generator here is to produce fake images that look real enough to fool the discriminator. 
So, let's talk about the Handwritten Digits  MNIST Dataset. This dataset contains 60,000 handwritten digits written on a whiteboard of size 28x28x1 labeled as their original values. What this model does is take an input seed of a one-dimensional array of size 100 random numbers and the generator learns from the dataset to create handwritten digits. The Discriminator, on the other hand, takes half the batch size of input as the rel images and the other half as the generated images and tries to classify them as real or fake.
One thing important to understand here is that the generator and the discriminator do not train simultaneously; they train separately. 
After training the dataset on 10,000 epochs, these were the results that I got. The digits generated are fairly readable other than some random noise which I believe would get removed if I trained it for more epochs
![mnist_9000](https://github.com/roseredfingers/Handwritten-Digits-GANs/assets/88833560/e39f829f-6326-42da-bbd8-f2157c85e696)

