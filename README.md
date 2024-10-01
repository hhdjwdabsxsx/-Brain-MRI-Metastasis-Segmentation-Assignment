# -Brain-MRI-Metastasis-Segmentation-Assignment
This project demonstrates the application of computer vision techniques for brain metastasis segmentation using two advanced architectures: Nested U-Net and Attention U-Net. These architectures are implemented to perform accurate segmentation of metastasis regions in brain MRI scans. The project also includes a web application for showcasing the model.

U-Net with Nested Structures
An improvement on the original U-Net architecture, the Nested U-Net (also known as U-Net++) is intended to enhance semantic segmentation tasks. At various stages of the encoder-decoder construction, it adds dense connections between layers. Among the primary enhancements are:
Dense skip connections: By directly connecting encoder layers to decoder layers at various sizes, they minimize information loss and aid in the preservation of spatial information.
Deep Supervision: The model's intermediate layers are supervised, which enhances the model's capacity to learn at different feature extraction levels.

Nested U-Net is helpful for metastatic segmentation because metastasis regions might vary in size and disperse across the brain. Accurately segmenting these diverse locations depends on capturing both fine and coarse data, which is made possible by the thick connections in Nested U-Net.

U-Net, take notice
The classic U-Net model gains attention mechanisms from the Attention U-Net design. The network may concentrate on significant portions of the image while disregarding unimportant ones thanks to this attention mechanism. Crucial elements consist of:

Greetings, Gates: These let the model concentrate on metastatic regions throughout the segmentation phase by dynamically suppressing unnecessary parts in the input.
Better Feature Depiction: The model may more accurately distinguish between background and metastasis when it focuses on certain locations, particularly when the metastatic regions are tiny or hard to detect.

Setup and Installation
Requirements
Python 3.7+
TensorFlow 2.0+
OpenCV
NumPy
scikit-learn
Flask (for web app)
Other dependencies as listed in requirements.txt



