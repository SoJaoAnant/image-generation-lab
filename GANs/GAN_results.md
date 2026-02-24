### Vanilla GAN
The Generator and The Discriminator had to be tweaked a lot because of the discriminator getting too powerful too easily and not letting the generator learn properly, so the discriminator had to be purposefully weakened by decrease in learning rate, having noise in its images and the generator training 3 more times than the discriminator.

Before, when the discriminator was bullying our generator, this is what the loss plot looked like, we can see the generator's loss increasing a lot
and the results dont quite look like what one was supposed to generate, the images of flowers.

##### Loss
<img src="Images and Examples/vgan_loss.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="Images and Examples/vgan_res.png" width="400">

After, when many tweaks were done, everything finally stablized and the training loop looked pretty promising, the generator was stable and was finally learning.

##### Loss
<img src="Images and Examples/vgan_loss_2.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="Images and Examples/vgan_res_1.png" width="400">
<img src="Images and Examples/vgan_res_2.png" width="400">

### Wasetterian GAN with Gradient Penalty
This is an advanced version of the vanilla GANs which uses the wasetterian distances to calculate its norm and uses graident penalty as a loss function to keep the gradients in control, so they dont leak above 1, which makes the training process significantly more stable.

The loss plot looked pretty stable and the results were absolutely amazing!
The images generated looks like they're photorealisic and are shot on some old camera 😄

##### Loss
<img src="Images and Examples/wgan_loss.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="Images and Examples/wgan_res.png" width="400">

### WGAN but with the dataset "Anime Faces"
I wanted to try something else, so the flower dataset was replaced by the anime faces dataset to see the outputs, and the results are again pretty amazing!

##### Loss
<img src="Images and Examples/wgan_anime_loss.png" width="400">

##### Results (Input images on top row and reconstructed on bottom)
<img src="Images and Examples/wgan_anime_res.gif" width="400">


With the learning of GANs aqquired, we move on to the state of the art trending models in the modern world, the diffusion models!




