## Face Generation using Deep Convolutional Generative Adversarial Network

This project is part of Udacity DLND. It is a Deep Convelutional Generative Adversarial Network trained on the CelebA dataset to generate new faces. The network is tested on MNIST dataset to generate digits.

# A quick challenge:
### Can you tell that which image below contains all real human faces and which contains all 'fake' faces generated by GAN?

<table style="width:100%">
  <tr>
    <th>
      <p align="center">
           <img src="./assets/ex1.jpeg"
           width="100%" height="80%">
           <br>Faces 1
      </p>
    </th>
    <th>
      <p align="center">
           <img src="./assets/ex2.jpeg"
           width="100%" height="80%">
           <br>Faces 2
      </p>
    </th>
  </tr>
 </table>
 
---


## Architecture

The architecture of DC-GAN contains a **generator** and a **discriminator**.

The generator used in the [original paper](https://arxiv.org/pdf/1511.06434.pdf):
![](https://github.com/Xfan1025/DLND-Face_Generation/blob/master/assets/dcgan.png)

I have reduced the number of units in the generator and reduced the number of layers for discriminator. I was still able to generate quite clear faces. So, if you got more computation power, you should try to make the network deeper to get better result.

Training loss of the network:

![](./assets/loss.png)

## CelebA
Trained after 7 epochs.

![](https://github.com/Xfan1025/DLND-Face_Generation/blob/master/assets/faces.gif)

## MNIST
I only trained it for 2 epochs. You should get better result if train it longer.

![](https://github.com/Xfan1025/DLND-Face_Generation/blob/master/assets/MNIST.gif)


