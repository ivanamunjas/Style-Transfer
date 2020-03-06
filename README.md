# Style Transfer

This project uses deep learning to compose images in the style of another image. This is known as style transfer and it was proposed in the following paper: [Leon A. Gatys’ paper, A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576).

Neural style transfer is an optimization technique used to take three images, a content image, a style reference image (such as an artwork by a famous painter), and the input image you want to style — and blend them together such that the input image is transformed to look like the content image, but “painted” in the style of the style image.

The principle of neural style transfer is to define two distance functions, one that describes how different the content of two images are, *Lcontent*, and one that describes the difference between the two images in terms of their style, *Lstyle*. Then, given three images, a desired style image, a desired content image, and the input image (initialized with the content image),the goal is to transform the input image to minimize the content distance with the content image and its style distance with the style image.
