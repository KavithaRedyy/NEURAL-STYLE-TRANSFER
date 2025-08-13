

# NEURAL-STYLE-TRANSFER

"Company name"=CODTECH IT SOLUTIONS

"Name"=Harivaram Naga Kavitha

"Domain"=Artificial Intelligence

"Duration"=6 weeks

"mentor name"= Neela Santosh

"Intern ID":CT06DZ2175

Neural Style Transfer (NST) is a computer vision technique that merges the content of one image with the style of another. It enables the transformation of a regular photograph into a stylized artwork by applying the visual appearance of a famous painting or artistic style. The underlying idea is to extract the content from one image and the style from another and then blend them using a deep learning model.

The technique is based on Convolutional Neural Networks (CNNs), particularly the VGG-19 architecture, which is pre-trained on a large dataset (like ImageNet) and known for its strong feature extraction capabilities. The NST process involves three primary images: the content image (e.g., a photo of a landscape), the style image (e.g., Van Gogh’s Starry Night), and the generated image, which starts as a copy of the content image and is updated iteratively to resemble the style image while preserving the content.

To achieve this, two types of losses are computed during training:

Content Loss: This measures the difference between the content image and the generated image at higher layers of the CNN, ensuring the structure and shapes remain recognizable.

Style Loss: This is calculated using the Gram matrix, which captures texture and style by comparing feature correlations in the style and generated images. It ensures the colors, brush strokes, and textures match the style image.

The process begins with loading and preprocessing the images. The images are resized, normalized, and converted into tensors for compatibility with the neural network. The VGG-19 model is then used to extract feature maps at various layers. These layers capture different levels of abstraction—lower layers represent edges and textures, while higher layers capture the image’s structure.

The NST model is then built by inserting content and style loss functions at specific layers of VGG-19. An optimization algorithm, typically L-BFGS, is used to update the pixels of the generated image based on the weighted sum of content and style losses. During each iteration, the model adjusts the generated image to better match the desired artistic style while retaining the original content.

The final output is a visually appealing image that artistically transforms the content image using the textures and colors of the style image. This can be used in creative fields like digital art, photo editing, game design, and filmmaking.

The deliverable for this project is a Python script or Jupyter Notebook that takes in a content image and a style image, applies neural style transfer, and outputs the stylized result. The implementation uses libraries such as PyTorch, Torchvision, PIL, and Matplotlib for deep learning, image processing, and visualization.


<img width="947" height="204" alt="image" src="https://github.com/user-attachments/assets/1214b089-de20-4d46-af53-ff944e44a77f" />

