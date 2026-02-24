### AutoEncoders using Multi Layered Perceptron
The Encoder and Decoder both were build using Multiple layers of perceptron, so the image was not interpreted as image but as an array of NxN values, yet,
The Decrease in Loss was slow and steady and the outputs were surprisingly good only with 10 epochs, yet one could pick out the faults and the details the decoder was unable to catch.

##### Loss
<img src="../imgs/ae_mlp_loss.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="../imgs/ae_mlp_res.png" width="400">


### AutoEncoders using Convolutional Neural Networks
The Encoders and Decoders both were now built using CNNs, the building block when working with images, thus it was to no surprise that the decrease in loss looked like an exponential decrease with just 1 epochs, and the loss stayed stagnant for its other 9 epochs.
The results are quite good too!

##### Loss
<img src="imgs/ae_cnn_loss.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="imgs/ae_cnn_res.png" width="400">


### Variational AutoEncoders
The only downside of AEs are that they can only reconstruct images but not create anything new, thus to beat those allegations, Variational AEs instead of representing and reconstructing the images as latent vectors, instead use latent distributions. The concept was pretty hard to grasp on, but with the results, it became all clear.
The Decrease in Loss was good and the outputs were absolutely mind opening, to see a gaussian distribution of numerical digits and how the model would interpret it.

##### Loss
<img src="imgs/vae_loss.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="imgs/vae_res.png" width="400">


With this, a good learning experience about the foundation of image generation was achieved and a path towards the more advanced and the successor models started. 