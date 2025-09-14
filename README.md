# Dogs vs Cats 

## History
The "Dogs vs. Cats" dataset has its roots in the Asirra project (Animal Species Image Recognition for Restricting Access), originally developed and implemented by Microsoft Research as a CAPTCHA system in 2007. Asirra challenged users to distinguish cats from dogs in photographs, a task that is trivial for humans but historically difficult for computers. Through a partnership with Petfinder.com, over three million manually classified cat and dog images were collected, providing one of the earliest large-scale image datasets for machine learning. 

## Present
This legacy evolved into the modern "Dogs vs. Cats" dataset, which is now a popular benchmark for image classification tasks, particularly for training Convolutional Neural Networks (CNNs). In practice, models are often trained on organized subsets of the data (in this case: 5,000 cats and 5,000 dogs) drawn from a larger dataset of 17,500 images containing photos of 8,750 cats and 8,750 dogs. This model utilizes a combination of advanced tools to learn visual features, evaluate and visualize predictions, and display final accuracy results (with performance analytics measured using Confusion Matrix and AUC/ROC Scores).

The following Python libraries & Machine Learning franeworks were employed to accurately differentiate whether an image is a cat or a dog:

### Open-Source Libraries
 - #### **NumPy** (for numerical array-based data preprocessing)  
 - #### **Matplotlib, Seaborn & PIL** (for displaying images and making the model’s performance visually-interpretable, not just numerically)
 - #### **Scikit-Learn** (for evaluate model predictions and quantify accuracy)

### Proprietary Machine Learning Frameworks 
 - #### **TensorFlow/Keras** (for loading, preprocessing, resizing images into the correct CNN input format for model architecture modeling)
 - #### **VGG-16** (pre-trained, deep CNN model - for feature extraction and transfer learning) 


## TensorFlow/Keras
Developed by Google, TensorFlow is a comprehensive open-source platform for machine learning, while Keras is its high-level API designed to simplify the building and training of neural networks. Developed by a French software engineer: (François Chollet), Keras has an intuitive, user-friendly interface to define deep learning models, making it easier to experiment quickly and develop complex architectures. It is fully integrated into TensorFlow as "tf.keras", allowing users to seamlessly leverage TensorFlow’s scalability and performance features. Essentially, TensorFlow serves as the powerful engine underneath, while Keras acts as a high-level API that reduces complexity and enhances productivity in model development.

## VGG-16 
VGG-16 is a deep convolutional neural network architecture developed by the Visual Geometry Group at the University of Oxford, consisting of 16 layers (including 13 convolutional layers and 3 fully-connected layers). The machine learning tools commonly used in implementing VGG-16 include TensorFlow and Keras, which provide the underlying framework for building and training the convolutional neural network models. VGG-16 uses small 3x3 convolutional filters stacked sequentially, with max-pooling layers for downsampling, and employs ReLU activation functions throughout. Designed for image classification, it takes 224x224 RGB images as input and outputs probabilities across 1,000 classes (achieving around 92.7% top-5 accuracy on the ImageNet dataset). Renowned for its simplicity, uniform architecture, and effectiveness, VGG-16 is widely used for deep learning applications and transfer learning.

VGG networks are designed, inspired by, and functionally analogous to the mammalian visual cortexwi (with layered feature hierarchies mirroring the brain's progression from simple to complex visual processing stages). Both systems filter visual data through multiple layers, progressively extracting more and more complex features as the signal moves deeper. Early layers in VGG networks resemble simple processing stages similar to those in the primary visual cortex (V1), which respond to basic features like edges and textures. Later-stage layers in VGG networks correspond to more abstract and complex feature representations akin to higher visual cortical areas, which integrate and interpret more detailed aspects of visual stimuli. Studies comparing VGG16 with the mouse visual cortex show that the intermediate layers of VGG correspond roughly to mid-level visual processing in the brain, indicating the representations are higher-order than simple edge detection. Additionally, unlike the strictly hierarchical feedforward nature of VGG, the mammalian visual cortex may exhibit a more parallel and broader organization beyond early visual areas. (Shi J, et al.)



### Acknowledgements

 - Special thanks to Professors Zia Khan & Frank Fletcher for their mentorship and code reviews. Thanks to the Microsoft Research team for providing the photographic data.

 - Additional thanks to LearningFuze and the open source community for continuous support and helpful discussions.

### Citations

 - Shi, J. et al. (2022) MouseNet: A biologically constrained convolutional neural network model for the Mouse Visual Cortex, PLoS computational biology. Available at: [(https://pubmed.ncbi.nlm.nih.gov/36067234/)]
(Accessed: 13 May 2025). 
 - Jeremy Elson, John R. Douceur, Jon Howell, Jared Saul, Asirra: A CAPTCHA that Exploits Interest-Aligned Manual Image Categorization, in Proceedings of 14th ACM Conference on Computer and Communications Security (CCS), Association for Computing Machinery, Inc., Oct. 2007.
