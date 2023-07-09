# Demystify Generative AI

“Technology advanced enough is indistinguishable from magic.”

--Arthur C. Clarke (author of 2001: A Space Odyssey)


## text, music, image, figure, and pattern generation in PyTorch

A 16-chapter series to create images, text, music, figures, and patterns in PyTorch. The series show how to:

* Create a ChatGPT-style large language model from scratch to generate text that can pass as human-written
* Generate images that are indistinguishable from real photos
* Compose music that anyone would think it’s real
* Create patterns such as a sequence of odd numbers, multiples of five, ...
* Generate data that mimic certain shapes: sine curve, cosine shape, hyperbola graph
* Control the latent space to generate images with certain attributes: men with glasses, women with glasses, transitioning gradually from men with glasses to men without glasses, or from women without glases to women with glasses...
* Style transfer: convert a horse image to a zebra... 

## Chapter 1: Introduction to PyTorch
## Chapter 2: Deep Learning with PyTorch
## Chapter 3: Generative Adversarial Networks (GANs)
Most of the generative models in this book belong to a framework called Generative Adversarial Networks (GANs). This chapter introduces you to the basic idea behind GANs and you'll learn to use the framework to generate data samples that form an inverted-U shape. At the end of this chapter, you'll be able to generate data to mimic any shape: sine, cosine, quadratic, and so on. 
![invertedU](https://github.com/markhliu/DGAI/assets/50116107/9da4fdab-d852-4f9e-b6bf-a184928d2885)

## Chapter 4: Pattern Generation with GANs
You'll learn how to use GAN to generate a sequence of numbers with certain patterns. We'll try to generate multiples of five. But you can change the pattern to multiples of two, three, seven, or any number really. This is the output from a trained GAN:

tensor([25,  0, 30, 40, 25, 35, 10, 30, 10,  0], device='cuda:0')

All numbers are multiples of five!

## Chapter 5: Image Generation with GANS
Generate image without using convolutional layers:

![imageGAN](https://github.com/markhliu/DGAI/assets/50116107/7aedad50-5393-4e91-8a23-1cc7409284ef)

## Chapter 6: High Resolution Image Generation with Deep Convolutional GANs
Use deep convolutional GAN to generate color images:

![anime](https://github.com/markhliu/DGAI/assets/50116107/273bda1e-3319-4009-9496-b17e382f0320)

and control attributes: here you can transition from red-hair to black-hair:

![attribute](https://github.com/markhliu/DGAI/assets/50116107/8e123398-111a-41c9-b9d2-5d977ec6a1a2)

## Chapter 7: Conditional GAN and Wasserstein GAN
Use Wasserstein distance to stabilize training, plus add label to generate certain types of images. E.g., faces without glasses over the course of training: 
https://gattonweb.uky.edu/faculty/lium/ml/noglasses.gif"
## Chapter 8: CycleGAN
Convert horses to zebras:

![Fz9kR4BakAEtZEU](https://github.com/markhliu/DGAI/assets/50116107/eb954b98-5fd5-45ae-81f1-03a8072efcd2)

## Chapter 9: Introduction to Variational Autoencoders
## Chapter 10: Attribute-Control in Variational Autoencoders
Train a variational autoencoder (VAE) to generate color images of human faces. Control encodings to generate images with certain attributes: e.g., images that gradually transition from images with glasses to images without glasses. Take the encodings of men with glasses, minus encodings of men without glasses, and add in the encodings of women without glasses, you'll generate images of women with glasses. The whole experience seems like straight out of science fiction, hence the opening quote by the science fiction writer Arthur Clarke: “Technology advanced enough is indistinguishable from magic.” 

To give you an idea what the chapter will accomplish, here is the transition from women with glasses to women without glasses:
<img src="https://gattonweb.uky.edu/faculty/lium/ml/wgwng6.png" />
Transition from women without glasses to men without glasses
<img src="https://gattonweb.uky.edu/faculty/lium/ml/wngmng6.png" />
Two examples of encoding arithmetic:
<img src="https://gattonweb.uky.edu/faculty/lium/ml/vectorArithmetic1.png" />

<img src="https://gattonweb.uky.edu/faculty/lium/ml/vectorArithmetic2.png" />


## Chapter 11: Text Generation with Character-Level LSTM
## Chapter 12: Text Generation with Word-Level LSTM
## Chapter 13: Create A GPT from Scratch
## Chapter 14: Train a ChatGPT style Transformer
## Chapter 15: MuseGAN
Train a generative adversarial network (GAN) to produce music. here is a sample of the generated music:
https://gattonweb.uky.edu/faculty/lium/ml/MuseGAN_song.mp3

## Chapter 16: Music Transformer
Train a ChatGPT-style transformer to generate music. here is a sample of the generated music:
https://gattonweb.uky.edu/faculty/lium/ml/musicTrans.mp3





