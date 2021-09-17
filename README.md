## StyleTransfer
Style transfer is a technique where we use two images 
- Content image which is the main content of the image
- Style image which could be termed as the layout of the image, something like a color scale in simplest of the terms

What style transfer does is that it takes the content of the content image and the style of the style image and merges them up to create an new image that resembles the content of the content image and the style of the style image

## CNN to capture the style and content of image
CNNs as we know are really awesome in detecting the representation of an image. An initial layer could detect just an edge of an image but as we go deeper it learns to detect even more complex structure of an image making it really useful for our purpose. For capturing the style and content of an image I have used the pretrained VGG19 network and extracted the features from the layers (conv1_1, conv2_1, conv3_1, conv4_1, conv5_1) respectively for both the style and the content although the paper does mention using second filters for the content image but the results were pretty similar
