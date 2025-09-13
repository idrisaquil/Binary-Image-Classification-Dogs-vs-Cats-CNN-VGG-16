# Dogs vs Cats 

The "Dogs vs. Cats" dataset is a popular benchmark for image classification tasks, particularly for learning Convolutional Neural Networks (CNNs). It involves training a model to distinguish between images of dogs and cats, often using a subset (in this case: 3,750 cats and 3,750 dogs) of a larger dataset. The larger dataset contains 17,500 images (8,750 cats and 8,750 dogs). Ultimately, creating a function or dataset that has an image name (or an image) that recognizes if image is cat or dog. Accuracy is measured via AUC/ROC Scores and Confusion Matrix

This project makes use of the following Python libraries & Machine Learning tools: 
 - #### **NumPy** (for data preprocessing) 
 - #### **Scikit-Learn** (for evaluate model predictions and quantify accuracy) 
 - #### **Matplotlib, Seaborn & PIL** (for displaying images and making the model’s performance visually-interpretable, not just numerically)

 - #### **TensorFlow/Keras** (for loading, preprocessing, resizing images into the correct CNN input format for model architecture modeling)
 - #### **VGG-16** (pre-trained, deep CNN model - for feature extraction and transfer learning) 

## NumPy
Short for Numerical Python, NumPy is an open-source Python library essential for large-scale numerical computing. It is written in low-level languages like C and provides powerful multi-dimensional array objects ("ndarrays") that enable an efficient storage and manipulation of large datasets. NumPy has a rich collection of higher mathematical functions for dataset tasks that utilize linear algebra, Fourier transforms, and statistical analysis; it is a cornerstone tool in scientific computing, data science, and machine learning. Its library arrays are stored in contiguous memory locations for fast computation and support vectorized operations, broadcasting, and advanced indexing to simplify code and enhance performance.


## TensorFlow/Keras
Developed by Google, TensorFlow is a comprehensive open-source platform for machine learning, while Keras is its high-level API designed to simplify the building and training of neural networks. Developed by a French software engineer: (François Chollet), Keras has an intuitive, user-friendly interface to define deep learning models, making it easier to experiment quickly and develop complex architectures. It is fully integrated into TensorFlow as "tf.keras", allowing users to seamlessly leverage TensorFlow’s scalability and performance features. Essentially, TensorFlow serves as the powerful engine underneath, while Keras acts as a high-level API that reduces complexity and enhances productivity in model development.


## VGG-16 
VGG-16 is a deep convolutional neural network architecture developed by the Visual Geometry Group at the University of Oxford, consisting of 16 layers, including 13 convolutional layers and 3 fully-connected layers. The machine learning tools commonly used in implementing VGG-16 include TensorFlow and Keras, which provide the underlying framework for building and training the convolutional neural network models. VGG-16 uses small 3x3 convolutional filters stacked sequentially, with max-pooling layers for downsampling, and employs ReLU activation functions throughout. Designed for image classification, it takes 224x224 RGB images as input and outputs probabilities across 1000 classes, achieving around 92.7% top-5 accuracy on the ImageNet dataset. Renowned for its simplicity, uniform architecture, and effectiveness, VGG-16 remains widely used for deep learning applications and transfer learning.

Essentially, VGG networks are designed inspired by and functionally analogous to the mammalian visual cortex, with layered feature hierarchies mirroring the brain's progression from simple to complex visual processing stages. Both systems process visual data through multiple layers, progressively extracting more complex features as the signal moves deeper. Early layers in VGG resemble simple processing stages similar to those in the primary visual cortex (V1), which respond to basic features like edges and textures. Later-stage layers in VGG correspond to more abstract and complex feature representations akin to higher visual cortical areas, which integrate and interpret more detailed aspects of visual stimuli. Studies comparing VGG16 with the mouse visual cortex show that the intermediate layers of VGG correspond roughly to mid-level visual processing in the brain, indicating the representations are higher-order than simple edge detection. Additionally, unlike the strictly hierarchical feedforward nature of VGG, the mammalian visual cortex may exhibit a more parallel and broader organization beyond early visual areas. 



### Acknowledgements

 - Special thanks to Professors Zia Khan & Frank Fletcher for their mentorship and code reviews. Thanks to the Microsoft Research team for providing the photographic data. The conceptual inspiration derives from the following publication:

   Jeremy Elson, John R. Douceur, Jon Howell, Jared Saul, Asirra: A CAPTCHA that Exploits Interest-Aligned Manual Image Categorization, in Proceedings of 14th ACM Conference on Computer and Communications Security (CCS), Association for Computing Machinery, Inc., Oct. 2007.

 - Thanks also to the LearningFuze and the open source community for continuous support and helpful discussions.
