# NEURAL-STYLE-TRANSFER
COMPANY : ``CODTECH IT SOLUTIONS

NAME : ANUSHA S

INTERN ID :CT04DH1155

DOMAIN : ARTIFICIAL INTELLIGENCE

DURATION : 4 WEEKS

MENTOR : NEELA SANTHOSH

DESCRIPTION : 
Neural Style Transfer (NST) is a cutting-edge deep learning application that creatively combines the content of one image with the artistic style of another. This project implements neural style transfer using Python and the PyTorch framework, offering users an interactive way to turn ordinary photos into artistic masterpieces. The concept behind NST is inspired by the human brain’s ability to distinguish between the content of an image (such as a person, object, or scene) and its style (such as brush strokes, color patterns, and textures). Using this technique, we can create a new image that preserves the recognizable structure of a "content image" while applying the visual aesthetic of a "style image"—for example, transforming a selfie into a painting that looks like it was done by Vincent van Gogh.

The core of this project relies on a pre-trained **VGG-19 Convolutional Neural Network**, which is known for its strong feature extraction abilities. Instead of training a new model from scratch, this project uses VGG-19 as a feature extractor to capture both low-level textures and high-level structures from the content and style images. The content image is passed through certain deeper layers of the network to capture its main features, while the style image is passed through shallower layers to collect stylistic elements. To represent the style mathematically, we compute the **Gram matrix** of the feature maps. This matrix captures the correlations between the different filters applied during convolution, helping us preserve the texture and style of the style image.

In the process, we define two loss functions: content loss and style loss. Content loss ensures that the output image stays similar in structure to the original content image. Style loss ensures that the output image mimics the artistic elements of the style image. The combination of these two losses, with adjustable weights, allows us to fine-tune how much "style" vs "content" is preserved in the final image. Instead of adjusting the weights of the network, as in typical training, we optimize the **pixels of the output image itself**. This means we start with a random or copied image and adjust it gradually so that it minimizes the total loss.

The entire pipeline is built to be simple and modular. The project includes clear functions for loading and preprocessing images, extracting features, computing Gram matrices, defining loss functions, and optimizing the output. While the project is CPU-compatible, using a GPU (if available) speeds up the training significantly. Once the output image is generated, it is de-normalized and displayed or saved. Users can experiment with different style-content image pairs, different style weights, and different optimization settings to see how the final results vary.

This project serves as both a technical and creative tool. From a technical perspective, it deepens understanding of how convolutional neural networks work, how transfer learning can be used, and how optimization can be applied in unusual contexts. From a creative perspective, it provides a fun way to blend photography with digital art. This approach has practical applications in photography apps, filter creation, and art generation. Additionally, it's an excellent project for students and enthusiasts wanting to explore machine learning beyond typical classification tasks. The project also lays the foundation for extending the concept into video style transfer or real-time mobile applications using more advanced models like Fast Neural Style Transfer.

Overall, this Neural Style Transfer project is a great mix of theory, creativity, and practical implementation. It gives users a hands-on opportunity to explore the fusion of art and AI, and produces visually stunning results from just a few lines of code. Whether you're a beginner learning about neural networks or a developer building creative tools, this project is an inspiring entry point into the world of AI-powered art.


